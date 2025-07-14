

- Vision
-  VNRequestRevisionProviding 

Protocol

# VNRequestRevisionProviding

A protocol for specifying the revision number of Vision algorithms.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
protocol VNRequestRevisionProviding
```

## Overview

Subclasses of VNRequest should adopt this protocol to specify which revision of an algorithm the Vision framework uses to generate requests.

## Topics

### Specifying Revision Number

var requestRevision: Int

The revision of the VNRequest subclass used to generate the implementing object.

**Required**

### Determining Revision Type

let VNRequestRevisionUnspecified: Int

A constant for specifying an unspecified request revision.

let VNDetectRectanglesRequestRevision1: Int

A constant for specifying revision 1 of the rectangle detection request.

let VNTrackRectangleRequestRevision1: Int

A constant for specifying revision 1 of the rectangling tracking request.

let VNTrackObjectRequestRevision1: Int

A constant for specifying revision 1 of the object tracking request.

let VNDetectFaceRectanglesRequestRevision2: Int

A constant for specifying revision 2 of the face rectangles detection request.

let VNDetectFaceRectanglesRequestRevision1: Int

A constant for specifying revision 1 of the face rectangles detection request.

Deprecated

let VNDetectFaceLandmarksRequestRevision3: Int

A constant for specifying revision 3 of the face landmarks detection request.

let VNDetectFaceLandmarksRequestRevision2: Int

A constant for specifying revision 2 of the face landmarks detection request.

let VNDetectFaceLandmarksRequestRevision1: Int

A constant for specifying revision 1 of the face landmarks detection request.

Deprecated

let VNRecognizeTextRequestRevision1: Int

A constant for specifying revision 1 of the text recognition request.

Deprecated

let VNDetectTextRectanglesRequestRevision1: Int

A constant for specifying revision 1 of the text rectangles detection request.

let VNDetectBarcodesRequestRevision1: Int

A constant for specifying revision 1 of the barcode detection request.

Deprecated

let VNDetectHorizonRequestRevision1: Int

A constant for specifying revision 1 of the horizon detection request.

let VNTranslationalImageRegistrationRequestRevision1: Int

A constant for specifying revision 1 of the translational image registration request.

let VNHomographicImageRegistrationRequestRevision1: Int

A constant for specifying revision 1 of the homographic image registration request.

let VNCoreMLRequestRevision1: Int

A constant for specifying revision 1 of a Core ML request.

let VNGenerateAttentionBasedSaliencyImageRequestRevision1: Int

A constant for specifying revision 1 of the image saliency request.

let VNGenerateObjectnessBasedSaliencyImageRequestRevision1: Int

A constant for specifying revision 1 of the image saliency request.

let VNClassifyImageRequestRevision1: Int

A constant for specifying the first revision of the image-classification request.

let VNGenerateImageFeaturePrintRequestRevision1: Int

A constant for specifying the first revision of the feature-print request.

let VNDetectFaceCaptureQualityRequestRevision1: Int

A constant for specifying revision 1 of the face capture detection request.

let VNDetectHumanRectanglesRequestRevision1: Int

A constant for specifying revision 1 of the human rectangles detection request.

## Relationships

### Conforming Types

- VNAnimalBodyPoseObservation
- VNBarcodeObservation
- VNClassificationObservation
- VNContour
- VNContoursObservation
- VNCoreMLFeatureValueObservation
- VNDetectedObjectObservation
- VNFaceLandmarkRegion
- VNFaceLandmarkRegion2D
- VNFaceLandmarks
- VNFaceLandmarks2D
- VNFaceObservation
- VNFeaturePrintObservation
- VNHorizonObservation
- VNHumanBodyPose3DObservation
- VNHumanBodyPoseObservation
- VNHumanHandPoseObservation
- VNHumanObservation
- VNImageAestheticsScoresObservation
- VNImageAlignmentObservation
- VNImageHomographicAlignmentObservation
- VNImageTranslationAlignmentObservation
- VNInstanceMaskObservation
- VNObservation
- VNPixelBufferObservation
- VNRecognizedObjectObservation
- VNRecognizedPoints3DObservation
- VNRecognizedPointsObservation
- VNRecognizedText
- VNRecognizedTextObservation
- VNRectangleObservation
- VNSaliencyImageObservation
- VNTextObservation
- VNTrajectoryObservation

## See Also

### Determining the Revision

class var currentRevision: Int

The current revison supported by the request.

class var defaultRevision: Int

The revision of the latest request for the particular SDK linked with the client application.

class var supportedRevisions: IndexSet

The collection of currently-supported algorithm versions for the class of request.

