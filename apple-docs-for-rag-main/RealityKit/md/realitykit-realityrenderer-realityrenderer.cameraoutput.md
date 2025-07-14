

- RealityKit
- RealityRenderer
-  RealityRenderer.CameraOutput 

Structure

# RealityRenderer.CameraOutput

Output produced by rendering with a camera.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct CameraOutput
```

## Topics

### Structures

struct Descriptor

Describes the output of rendering with a camera.

struct RelativeViewport

Structure defining a viewport for rendering with a camera.

### Initializers

init(RealityRenderer.CameraOutput.Descriptor) throws

Create a new output instance for rendering with a camera.

### Instance Properties

var colorTextures: [any MTLTexture]

Textures to store color output.

var viewports: [RealityRenderer.CameraOutput.RelativeViewport]

Viewports to use for rendering with a camera.

## See Also

### Metal workflow rendering

class RealityRenderer

A renderer that displays a RealityKit scene in an existing Metal workflow.

struct CameraSettings

Settings for rendering with a camera.

struct ImageBasedLight

Describe the lighting properties for the scene.

struct MetalEventAction

The structure describing an event and value to be signaled or waited for.

struct EntityCollection

A collection of entities in a RealityRenderer.

