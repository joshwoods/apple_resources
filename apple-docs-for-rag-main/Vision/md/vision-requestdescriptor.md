

- Vision
-  RequestDescriptor 

Enumeration

# RequestDescriptor

A type that describes the request and revision combination.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum RequestDescriptor
```

## Topics

### Getting the still-image descriptor

case classifyImageRequest(ClassifyImageRequest.Revision)

A descriptor that describes a classify image request.

### Getting the image sequence descriptor

case detectDocumentSegmentationRequest(DetectDocumentSegmentationRequest.Revision)

A descriptor that describes a detect document segmentation request.

case generatePersonInstanceMaskRequest(GeneratePersonInstanceMaskRequest.Revision)

A descriptor that describes a generate person instance mask request.

case generatePersonSegmentationRequest(GeneratePersonSegmentationRequest.Revision)

A descriptor that describes a generate person segmentation request.

### Getting the image aesthetics descriptor

case calculateImageAestheticsScoresRequest(CalculateImageAestheticsScoresRequest.Revision)

A descriptor that describes a calculate image aesthetics scores request.

### Getting the saliency descriptor

case generateAttentionBasedSaliencyImageRequest(GenerateAttentionBasedSaliencyImageRequest.Revision)

A descriptor that describes a generate attention based saliency image request.

case generateObjectnessBasedSaliencyImageRequest(GenerateObjectnessBasedSaliencyImageRequest.Revision)

A descriptor that describes a generate objectness based saliency image request.

### Getting the object-tracking descriptor

case trackObjectRequest(TrackObjectRequest.Revision)

A descriptor that describes a track object request.

case trackRectangleRequest(TrackRectangleRequest.Revision)

A descriptor that describes a track rectangles request.

### Getting the face and body detection descriptor

case detectFaceCaptureQualityRequest(DetectFaceCaptureQualityRequest.Revision)

A descriptor that describes a detect face capture quality request.

case detectFaceLandmarksRequest(DetectFaceLandmarksRequest.Revision)

A descriptor that describes a detect face landmarks request.

case detectFaceRectanglesRequest(DetectFaceRectanglesRequest.Revision)

A descriptor that describes a detect face rectangles request.

case detectHumanRectanglesRequest(DetectHumanRectanglesRequest.Revision)

A descriptor that describes a detect human rectangles request.

### Getting the body and hand pose detection descriptor

case detectHumanBodyPoseRequest(DetectHumanBodyPoseRequest.Revision)

A descriptor that describes a detect human body pose request.

case detectHumanHandPoseRequest(DetectHumanHandPoseRequest.Revision)

A descriptor that describes a detect human hand pose request.

case detectHumanBodyPose3DRequest(DetectHumanBodyPose3DRequest.Revision)

A descriptor that describes a 3D detect human body pose request.

### Getting the animal detection descriptor

case detectAnimalBodyPoseRequest(DetectAnimalBodyPoseRequest.Revision)

A descriptor that describes a detect animal body pose request.

case recognizeAnimalsRequest(RecognizeAnimalsRequest.Revision)

A descriptor that describes a recognize animals request.

### Getting the text descriptor

case detectTextRectanglesRequest(DetectTextRectanglesRequest.Revision)

A descriptor that describes a detect text rectangles request.

case recognizeTextRequest(RecognizeTextRequest.Revision)

A descriptor that describes a recognize text request.

### Getting the image alignment, feature print, and background removal descriptor

case trackTranslationalImageRegistrationRequest(TrackTranslationalImageRegistrationRequest.Revision)

A descriptor that describes a track translational image request.

case trackHomographicImageRegistrationRequest(TrackHomographicImageRegistrationRequest.Revision)

A descriptor that describes a track homographic image request.

case generateForegroundInstanceMaskRequest(GenerateForegroundInstanceMaskRequest.Revision)

A descriptor that describes a generate foreground instance mask request.

case generateImageFeaturePrintRequest(GenerateImageFeaturePrintRequest.Revision)

A descriptor that describes a generate image feature print request.

### Getting the trajectory, contour, and horizon detection descriptor

case detectTrajectoriesRequest(DetectTrajectoriesRequest.Revision)

A descriptor that describes a detect trajectories request.

case detectContoursRequest(DetectContoursRequest.Revision)

A descriptor that describes a detect contours request.

case detectHorizonRequest(DetectHorizonRequest.Revision)

A descriptor that describes a detect horizon request.

### Getting the optical flow, rectangle and barcode detection descriptor

case trackOpticalFlowRequest(TrackOpticalFlowRequest.Revision)

A descriptor that describes a track optical flow request.

case detectRectanglesRequest(DetectRectanglesRequest.Revision)

A descriptor that describes a detect rectangles request.

case detectBarcodesRequest(DetectBarcodesRequest.Revision)

A descriptor that describes a detect barcodes request.

### Getting the machine learning image-analysis descriptor

case coreMLRequest(CoreMLRequest.Revision)

A descriptor that describes a Core ML request.

## Relationships

### Conforms To

- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Inspecting an observation

var hasPrecisionRecallCurve: Bool

A Boolean value that indicates whether the observation contains precision and recall curves.

let identifier: String

The classification label that identifies the type of observation.

