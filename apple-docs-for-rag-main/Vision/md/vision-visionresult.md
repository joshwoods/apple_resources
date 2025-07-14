

- Vision
-  VisionResult 

Enumeration

# VisionResult

The result the framework produces by performing a request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum VisionResult
```

## Overview

Each result contains the original VisionRequest, along with any observations produced.

## Topics

### Getting the still-image result

case classifyImage(ClassifyImageRequest, [ClassificationObservation])

A result from performing a classify image request.

### Getting the image sequence result

case generatePersonInstanceMask(GeneratePersonInstanceMaskRequest, InstanceMaskObservation?)

A result from performing a generate person instance mask request.

case detectDocumentSegmentation(DetectDocumentSegmentationRequest, DetectedDocumentObservation?)

A result from performing a detect document segmentation request.

case generatePersonSegmentation(GeneratePersonSegmentationRequest, PixelBufferObservation)

A result from performing a generate person segmentation request.

### Getting the image aesthetics result

case calculateImageAestheticsScores(CalculateImageAestheticsScoresRequest, ImageAestheticsScoresObservation)

A result from performing a calculate image aesthetics scores request.

### Getting the saliency result

case generateObjectnessBasedSaliencyImage(GenerateObjectnessBasedSaliencyImageRequest, SaliencyImageObservation)

A result from performing a generate objectness based saliency image request.

case generateAttentionBasedSaliencyImage(GenerateAttentionBasedSaliencyImageRequest, SaliencyImageObservation)

A result from performing a generate attention based saliency image request.

### Getting the object-tracking result

case trackRectangle(TrackRectangleRequest, RectangleObservation?)

A result from performing a track rectangle request.

case trackObject(TrackObjectRequest, DetectedObjectObservation?)

A result from performing a track object request.

### Getting the face and body detection result

case detectFaceCaptureQuality(DetectFaceCaptureQualityRequest, [FaceObservation])

A result from performing a detect face capture quality request.

case detectFaceLandmarks(DetectFaceLandmarksRequest, [FaceObservation])

A result from performing a detect face landmarks request.

case detectFaceRectangles(DetectFaceRectanglesRequest, [FaceObservation])

A result from performing a detect face rectangles request.

case detectHumanRectangles(DetectHumanRectanglesRequest, [HumanObservation])

A result from performing a detect human rectangles request.

### Getting the body and hand pose detection result

case detectHumanBodyPose(DetectHumanBodyPoseRequest, [HumanBodyPoseObservation])

A result from performing a detect human body pose request.

case detectHumanHandPose(DetectHumanHandPoseRequest, [HumanHandPoseObservation])

A result from performing a detect human hand pose request.

case detectHumanBodyPose3D(DetectHumanBodyPose3DRequest, [HumanBodyPose3DObservation])

A result from performing a 3D detect human body pose request.

### Getting the animal detection result

case recognizeAnimals(RecognizeAnimalsRequest, [RecognizedObjectObservation])

A result from performing a recognize animals request.

case detectAnimalBodyPose(DetectAnimalBodyPoseRequest, [AnimalBodyPoseObservation])

A result from performing a detect animal body pose request.

### Getting the text result

case detectTextRectangles(DetectTextRectanglesRequest, [TextObservation])

A result from performing a detect text rectangles request.

case recognizeText(RecognizeTextRequest, [RecognizedTextObservation])

A result from performing a recognize text request.

### Getting the image alignment, feature print, and background removal result

case trackTranslationalImageRegistration(TrackTranslationalImageRegistrationRequest, ImageTranslationAlignmentObservation)

A result from performing a track translational image request.

case trackHomographicImageRegistration(TrackHomographicImageRegistrationRequest, ImageHomographicAlignmentObservation)

A result from performing a track homographic image request.

case generateForegroundInstanceMask(GenerateForegroundInstanceMaskRequest, InstanceMaskObservation?)

A result from performing a generate foreground instance mask request.

case generateImageFeaturePrint(GenerateImageFeaturePrintRequest, FeaturePrintObservation)

A result from performing a generate image feature print request.

### Getting the trajectory, contour, and horizon detection result

case detectTrajectories(DetectTrajectoriesRequest, [TrajectoryObservation])

A result from performing a detect trajectories request.

case detectContours(DetectContoursRequest, ContoursObservation)

A result from performing a detect contours request.

case detectHorizon(DetectHorizonRequest, HorizonObservation?)

A result from performing a detect horizon request.

### Getting the optical flow, rectangle and barcode detection result

case trackOpticalFlow(TrackOpticalFlowRequest, OpticalFlowObservation?)

A result from performing a track optical flow request.

case detectRectangles(DetectRectanglesRequest, [RectangleObservation])

A result from performing a detect rectangles request.

case detectBarcodes(DetectBarcodesRequest, [BarcodeObservation])

A result from performing a detect barcodes request.

### Getting the machine learning image-analysis result

case coreML(CoreMLRequest, [any VisionObservation])

A result from performing a Core ML request.

### Getting the error result

case error(any VisionRequest, any Error)

A result from encountering a framework error.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Sendable

## See Also

### Performing the request

associatedtype Result

An associated type that represents the result.

**Required**

