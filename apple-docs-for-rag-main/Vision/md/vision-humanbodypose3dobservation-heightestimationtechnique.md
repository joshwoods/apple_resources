

- Vision
- HumanBodyPose3DObservation
-  heightEstimationTechnique 

Instance Property

# heightEstimationTechnique

The technique the framework uses to estimate body height.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let heightEstimationTechnique: HumanBodyPose3DObservation.EstimationTechnique
```

## See Also

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

let bodyHeight: Measurement&lt;UnitLength>

The estimated human body height, in meters.

let cameraOriginMatrix: simd_float4x4

A transform from the skeleton hip to the camera.

enum EstimationTechnique

Constants that identify body height estimation techniques.

