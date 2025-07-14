

- Vision
-  QuadrilateralProviding 

Protocol

# QuadrilateralProviding

A protocol for objects that have a bounding quadrilateral.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
protocol QuadrilateralProviding : BoundingBoxProviding
```

## Topics

### Getting the normalized points

var bottomLeft: NormalizedPoint

The coordinates of the lower-left corner of the quadrilateral.

**Required**

var bottomRight: NormalizedPoint

The coordinates of the lower-right corner of quadrilateral.

**Required**

var topLeft: NormalizedPoint

The coordinates of the upper-left corner of the quadrilateral.

**Required**

var topRight: NormalizedPoint

The coordinates of the upper-right corner of the quadrilateral.

**Required**

## Relationships

### Inherits From

- BoundingBoxProviding

### Conforming Types

- BarcodeObservation
- DetectedDocumentObservation
- RecognizedTextObservation
- RectangleObservation
- TextObservation

## See Also

### Inspecting a request

let inputObservation: any QuadrilateralProviding &amp; VisionObservation

The object to track.

var trackingLevel: TrackRectangleRequest.TrackingLevel

The tracking quality preference.

enum TrackingLevel

