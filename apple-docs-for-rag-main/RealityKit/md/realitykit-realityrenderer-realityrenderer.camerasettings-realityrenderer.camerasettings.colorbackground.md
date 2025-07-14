

- RealityKit
- RealityRenderer
- RealityRenderer.CameraSettings
-  RealityRenderer.CameraSettings.ColorBackground 

Structure

# RealityRenderer.CameraSettings.ColorBackground

Defines the background

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct ColorBackground
```

## Topics

### Type Methods

static func color(CGColor) -> RealityRenderer.CameraSettings.ColorBackground

Use a solid color as background.

static func outputTexture() -> RealityRenderer.CameraSettings.ColorBackground

Use the corresponding `CameraOutput` colorTexture as background.

