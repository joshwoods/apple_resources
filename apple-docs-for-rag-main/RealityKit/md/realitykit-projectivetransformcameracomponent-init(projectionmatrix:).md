

- RealityKit
- ProjectiveTransformCameraComponent
-  init(projectionMatrix:) 

Initializer

# init(projectionMatrix:)

Creates a new custom matrix camera component with the given settings.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(projectionMatrix: float4x4)
```

## Parameters 

`projectionMatrix`  

The custom projection matrix the user wants to use.

## Discussion

The matrix uses reverse depth.

