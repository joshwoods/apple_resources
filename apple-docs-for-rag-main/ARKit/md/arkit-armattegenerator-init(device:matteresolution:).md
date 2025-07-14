

- ARKit
- ARMatteGenerator
-  init(device:matteResolution:) 

Initializer

# init(device:matteResolution:)

Creates an AR matte generator.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
init(
    device: any MTLDevice,
    matteResolution: ARMatteGenerator.Resolution
)
```

## Discussion

To create matte textures in real-time, create this object once and reuse it every frame.

