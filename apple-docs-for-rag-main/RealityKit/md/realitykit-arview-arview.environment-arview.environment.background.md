

- RealityKit
- ARView
- ARView.Environment
-  ARView.Environment.Background 

Structure

# ARView.Environment.Background

Content that appears as the background of the scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
struct Background
```

## Topics

### Backgrounds

static func cameraFeed(exposureCompensation: Float) -> ARView.Environment.Background

Use the camera feed as a background.

static func color(ARView.Environment.Color) -> ARView.Environment.Background

Use a solid color as a background.

static func color(ARView.Environment.Color) -> ARView.Environment.Background

Use a solid color as a background.

static func skybox(EnvironmentResource) -> ARView.Environment.Background

Use a skybox environment resource as a background.

## See Also

### Setting a background

var background: ARView.Environment.Background

The background for the environment.

