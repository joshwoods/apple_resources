

- RealityKit
- ARView
- ARView.Environment
- ARView.Environment.Background
-  cameraFeed(exposureCompensation:) 

Type Method

# cameraFeed(exposureCompensation:)

Use the camera feed as a background.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+

``` source
static func cameraFeed(exposureCompensation: Float = 0.0) -> ARView.Environment.Background
```

## Parameters 

`exposureCompensation`  

The exposure compensation used on the camera feed to lighten or darken it.

## See Also

### Backgrounds

static func color(ARView.Environment.Color) -> ARView.Environment.Background

Use a solid color as a background.

static func color(ARView.Environment.Color) -> ARView.Environment.Background

Use a solid color as a background.

static func skybox(EnvironmentResource) -> ARView.Environment.Background

Use a skybox environment resource as a background.

