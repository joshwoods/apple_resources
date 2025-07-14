

- Vision
- FaceObservation
-  landmarks 

Instance Property

# landmarks

The facial features of the detected face.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let landmarks: FaceObservation.Landmarks2D?
```

## Discussion

This value is `nil` for face observations produced by a DetectFaceRectanglesRequest analysis. Use the DetectFaceLandmarksRequest object to find facial features.

## See Also

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

struct Landmarks2D

A collection of facial features that a request detects.

let pitch: Measurement&lt;UnitAngle>

The pitch angle of a face.

let roll: Measurement&lt;UnitAngle>

The roll angle of a face.

let yaw: Measurement&lt;UnitAngle>

The yaw angle of a face.

