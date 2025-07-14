

- Vision
- FaceObservation
-  pitch 

Instance Property

# pitch

The pitch angle of a face.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let pitch: Measurement
```

## Discussion

This value indicates the rotational angle of the face around the x-axis.

## See Also

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

struct Landmarks2D

A collection of facial features that a request detects.

let landmarks: FaceObservation.Landmarks2D?

The facial features of the detected face.

let roll: Measurement&lt;UnitAngle>

The roll angle of a face.

let yaw: Measurement&lt;UnitAngle>

The yaw angle of a face.

