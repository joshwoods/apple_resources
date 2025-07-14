

- RealityKit
- RealityRenderer
- RealityRenderer.CameraOutput
-  RealityRenderer.CameraOutput.Descriptor 

Structure

# RealityRenderer.CameraOutput.Descriptor

Describes the output of rendering with a camera.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct Descriptor
```

## Topics

### Instance Properties

var colorTextures: [any MTLTexture]

Textures to store color output.

var viewports: [RealityRenderer.CameraOutput.RelativeViewport]

Viewports to use for rendering with a camera.

### Type Methods

static func singleProjection(colorTexture: any MTLTexture) -> RealityRenderer.CameraOutput.Descriptor

Creates a descriptor for single projection output.

