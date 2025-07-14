

- RealityKit
- RealityRenderer
-  RealityRenderer.CameraSettings 

Structure

# RealityRenderer.CameraSettings

Settings for rendering with a camera.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct CameraSettings
```

## Topics

### Structures

struct ColorBackground

Defines the background

### Instance Properties

var antialiasing: AntialiasingMode

var colorBackground: RealityRenderer.CameraSettings.ColorBackground

The background to use for rendering with a camera.

var isToneMappingEnabled: Bool

Specifies if tone mapping is enabled.

## See Also

### Metal workflow rendering

class RealityRenderer

A renderer that displays a RealityKit scene in an existing Metal workflow.

struct CameraOutput

Output produced by rendering with a camera.

struct ImageBasedLight

Describe the lighting properties for the scene.

struct MetalEventAction

The structure describing an event and value to be signaled or waited for.

struct EntityCollection

A collection of entities in a RealityRenderer.

