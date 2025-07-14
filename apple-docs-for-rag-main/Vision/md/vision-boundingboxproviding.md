

- Vision
-  BoundingBoxProviding 

Protocol

# BoundingBoxProviding

A protocol for objects that have a bounding box.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
protocol BoundingBoxProviding
```

## Topics

### Getting the bounding box

var boundingBox: NormalizedRect

The bounding box of the object.

**Required** Default implementation provided.

## Relationships

### Inherited By

- QuadrilateralProviding

### Conforming Types

- BarcodeObservation
- DetectedDocumentObservation
- DetectedObjectObservation
- FaceObservation
- HumanObservation
- RecognizedObjectObservation
- RecognizedTextObservation
- RectangleObservation
- TextObservation

## See Also

### Creating a request

init(detectedObject: any BoundingBoxProviding &amp; VisionObservation, TrackObjectRequest.Revision?, frameAnalysisSpacing: CMTime?)

Creates an object tracking request.

