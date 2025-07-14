

- Vision
- HumanBodyPose3DObservation
-  cameraOriginMatrix 

Instance Property

# cameraOriginMatrix

A transform from the skeleton hip to the camera.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let cameraOriginMatrix: simd_float4x4
```

## See Also

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

let bodyHeight: Measurement&lt;UnitLength>

The estimated human body height, in meters.

enum EstimationTechnique

Constants that identify body height estimation techniques.

let heightEstimationTechnique: HumanBodyPose3DObservation.EstimationTechnique

The technique the framework uses to estimate body height.

