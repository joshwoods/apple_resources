

- Core ML
- Model Integration Samples
-  Understanding a Dice Roll with Vision and Object Detection 

Sample Code

# Understanding a Dice Roll with Vision and Object Detection

Detect dice position and values shown in a camera frame, and determine the end of a roll by leveraging a dice detection model.

Download

iOS 13.0+iPadOS 13.0+Xcode 12.0+

## Overview

This sample app uses an object detection model trained with to recognize the tops of dice and their values when the dice roll onto a flat surface.

After you run the object detection model on camera frames through Vision, the model interprets the result to identify when a roll has ended and what values the dice show.

Note

This sample code project is associated with WWDC 2019 session 228: Creating Great Apps Using Core ML and ARKit.

### Configure the Sample Code Project

Before you run the sample code project in Xcode, note the following:

- You must run this sample code project on a physical device that uses iOS 13 or later. The project doesn’t work with Simulator.

- The model works best on white dice with black pips. It may perform differently on dice that use other colors.

### Add Inputs to the Request

In Vision, beginning in iOS 13, you can provide inputs other than images to a model by attaching an MLFeatureProvider object to your model. This is useful in the case of object detection when you want to specify different thresholds than the defaults.

As shown below, a feature provider can provide values for the `iouThreshold` and `confidenceThreshold` inputs to your object detection model.

class ThresholdProvider: MLFeatureProvider {
    /// The actual values to provide as input
    ///
    /// Create ML Defaults are 0.45 for IOU and 0.25 for confidence.
    /// Here the IOU threshold is relaxed a little bit because there are
    /// sometimes multiple overlapping boxes per die.
    /// Technically, relaxing the IOU threshold means
    /// non-maximum-suppression (NMS) becomes stricter (fewer boxes are shown).
    /// The confidence threshold can also be relaxed slightly because
    /// objects look very consistent and are easily detected on a homogeneous
    /// background.
    open var values = [
        &quot;iouThreshold&quot;: MLFeatureValue(double: 0.3),
        &quot;confidenceThreshold&quot;: MLFeatureValue(double: 0.2)
    ]

    /// The feature names the provider has, per the MLFeatureProvider protocol
    var featureNames: Set&lt;String> {
        return Set(values.keys)
    }

    /// The actual values for the features the provider can provide
    func featureValue(for featureName: String) -> MLFeatureValue? {
        return values[featureName]
    }
}

To use this threshold provider with your VNCoreMLModel, assign it to the featureProvider property of your VNCoreMLModel as seen in the following example.

### Set Up a Vision Request to Handle Camera Frames

For simplicity, you can use camera frames coming from an ARSession.

To run your detector on these frames, first set up a VNCoreMLRequest request with your model, as shown in the example below.

guard let mlModel = try? DiceDetector(configuration: .init()).model,
      let detector = try? VNCoreMLModel(for: mlModel) else {
    print(&quot;Failed to load detector!&quot;)
    return
}

// Use a threshold provider to specify custom thresholds for the object detector.
detector.featureProvider = ThresholdProvider()

diceDetectionRequest = VNCoreMLRequest(model: detector) { [weak self] request, error in
    self?.detectionRequestHandler(request: request, error: error)
}
// .scaleFill results in a slight skew but the model was trained accordingly
// see https://developer.apple.com/documentation/vision/vnimagecropandscaleoption for more information
diceDetectionRequest.imageCropAndScaleOption = .scaleFill

### Pass Camera Frames to the Object Detector to Predict Dice Locations

Pass the frames from the camera to the VNCoreMLRequest so it can make predictions using a VNImageRequestHandler object. The VNImageRequestHandler object handles image resizing and preprocessing as well as post-processing of your model’s outputs for every prediction.

To pass camera frames to your model, you first need to find the image orientation that corresponds to your device’s physical orientation. If the device’s orientation changes, the aspect ratio of the images can also change. Because you need to scale the bounding boxes for the detected objects back to your original image, you need to keep track of its size.

// The frame is always oriented based on the camera sensor,
// so in most cases Vision needs to rotate it for the model to work as expected.
let orientation = UIDevice.current.orientation

// The image captured by the camera
let image = frame.capturedImage

let imageOrientation: CGImagePropertyOrientation
switch orientation {
case .portrait:
    imageOrientation = .right
case .portraitUpsideDown:
    imageOrientation = .left
case .landscapeLeft:
    imageOrientation = .up
case .landscapeRight:
    imageOrientation = .down
case .unknown:
    print(&quot;The device orientation is unknown, the predictions may be affected&quot;)
    fallthrough
default:
    // By default keep the last orientation
    // This applies for faceUp and faceDown
    imageOrientation = self.lastOrientation
}

// For object detection, keeping track of the image buffer size
// to know how to draw bounding boxes based on relative values.
if self.bufferSize == nil || self.lastOrientation != imageOrientation {
    self.lastOrientation = imageOrientation
    let pixelBufferWidth = CVPixelBufferGetWidth(image)
    let pixelBufferHeight = CVPixelBufferGetHeight(image)
    if [.up, .down].contains(imageOrientation) {
        self.bufferSize = CGSize(width: pixelBufferWidth,
                                 height: pixelBufferHeight)
    } else {
        self.bufferSize = CGSize(width: pixelBufferHeight,
                                 height: pixelBufferWidth)
    }
}

Finally, you invoke the VNImageRequestHandler with the image from the camera and information about the current orientation to make a prediction using your object detector.

// Invoke a VNRequestHandler with that image
let handler = VNImageRequestHandler(cvPixelBuffer: image, orientation: imageOrientation, options: [:])

do {
    try handler.perform([self.diceDetectionRequest])
} catch {
    print(&quot;CoreML request failed with error: \(error.localizedDescription)&quot;)
}

Now that the app handles providing *input* data to your model, it’s time to interpret your model’s *output*.

### Draw Bounding Boxes to Understand Your Model’s Behavior

You can get a better understanding of how well your detector performs by drawing bounding boxes around each object and its text label. The dice detection model detects the tops of dice and labels them according to the number of pips shown on each die’s top side.

To draw bounding boxes, see Recognizing Objects in Live Capture.

### Determine When a Roll Has Ended

When playing a dice game, users want to know the result of a roll. The app determines that the roll has ended by waiting for the dice’s positions and values to stabilize.

You can define the requirements of an ended roll as a comparison between two consecutive camera frames with the following conditions:

- The number of detected dice must be the same.

- For each detected die:

  - The bounding box must have not moved.

  - The identified class must match.

Based on these constraints, you can make a function that tells the app whether a roll has ended based on the current and the previous VNRecognizedObjectObservation objects.

/// Determines if a roll has ended with the current dice values O(n^2)
///
/// - parameter observations: The object detection observations from the model
/// - returns: True if the roll has ended
func hasRollEnded(observations: [VNRecognizedObjectObservation]) -> Bool {
    // First check if same number of dice were detected
    if lastObservations.count != observations.count {
        lastObservations = observations
        return false
    }
    var matches = 0
    for newObservation in observations {
        for oldObservation in lastObservations {
            // If the labels don&#39;t match, skip it
            // Or if the IOU is less than 85%, consider this box different
            // Either it&#39;s a different die or the same die has moved
            if newObservation.labels.first?.identifier == oldObservation.labels.first?.identifier &amp;&amp;
                intersectionOverUnion(oldObservation.boundingBox, newObservation.boundingBox) > 0.85 {
                matches += 1
            }
        }
    }
    lastObservations = observations
    return matches == observations.count
}

Now for every prediction (meaning every new camera frame) you can check whether the roll has ended.

### Display the Dice Values

Once the roll has ended, you can display the information on the screen or trigger some other behavior in the setting of a game.

This sample app shows the list of recognized values on screen, sorted from left-most to right-most VNRecognizedObjectObservation. It sorts the values based on where the dice are on the surface according to each observation’s bounding box coordinates. The app does this by sorting the observations by their bounding box’s `centerX` property in ascending order.

var sortableDiceValues = [(value: Int, xPosition: CGFloat)]()

for observation in observations {
    // Select only the label with the highest confidence.
    guard let topLabelObservation = observation.labels.first else {
        print(&quot;Object observation has no labels&quot;)
        continue
    }

    if let intValue = Int(topLabelObservation.identifier) {
        sortableDiceValues.append((value: intValue, xPosition: observation.boundingBox.midX))
    }
}

let diceValues = sortableDiceValues.sorted { $0.xPosition &lt; $1.xPosition }.map { $0.value }

## See Also

### Object recognition

Recognizing Objects in Live Capture

Apply Vision algorithms to identify objects in real-time video.

class VNRecognizedObjectObservation

A detected object observation with an array of classification labels that classify the recognized object.

