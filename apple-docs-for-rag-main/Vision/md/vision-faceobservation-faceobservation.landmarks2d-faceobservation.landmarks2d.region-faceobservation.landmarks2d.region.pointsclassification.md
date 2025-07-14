

- Vision
- FaceObservation
- FaceObservation.Landmarks2D
- FaceObservation.Landmarks2D.Region
-  FaceObservation.Landmarks2D.Region.PointsClassification 

Enumeration

# FaceObservation.Landmarks2D.Region.PointsClassification

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum PointsClassification
```

## Topics

### Getting the point classifications

case closedPath

case disconnected

case openPath

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Inspecting a region

let originatingRequestDescriptor: RequestDescriptor?

let points: [NormalizedPoint]

let pointsClassification: FaceObservation.Landmarks2D.Region.PointsClassification

let precisionEstimatesPerPoint: [Float]?

