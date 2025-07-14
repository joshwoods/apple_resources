

- Vision
- FaceObservation
- FaceObservation.Landmarks2D
-  FaceObservation.Landmarks2D.Region 

Structure

# FaceObservation.Landmarks2D.Region

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct Region
```

## Topics

### Inspecting a region

let originatingRequestDescriptor: RequestDescriptor?

let points: [NormalizedPoint]

let pointsClassification: FaceObservation.Landmarks2D.Region.PointsClassification

enum PointsClassification

let precisionEstimatesPerPoint: [Float]?

### Getting the points

func pointsInImageCoordinates(CGSize, origin: CoordinateOrigin) -> [CGPoint]

## Relationships

### Conforms To

- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Getting all landmarks

var allPoints: FaceObservation.Landmarks2D.Region

