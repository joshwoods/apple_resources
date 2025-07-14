

- Vision
- FaceObservation
-  yaw 

Instance Property

# yaw

The yaw angle of a face.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let yaw: Measurement
```

## Discussion

This value indicates the rotational angle of the face around the y-axis.

## See Also

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

struct Landmarks2D

A collection of facial features that a request detects.

let landmarks: FaceObservation.Landmarks2D?

The facial features of the detected face.

let pitch: Measurement&lt;UnitAngle>

The pitch angle of a face.

let roll: Measurement&lt;UnitAngle>

The roll angle of a face.

