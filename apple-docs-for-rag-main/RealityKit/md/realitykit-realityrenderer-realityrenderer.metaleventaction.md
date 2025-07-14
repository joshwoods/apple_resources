

- RealityKit
- RealityRenderer
-  RealityRenderer.MetalEventAction 

Structure

# RealityRenderer.MetalEventAction

The structure describing an event and value to be signaled or waited for.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct MetalEventAction
```

## Topics

### Instance Properties

let event: any MTLEvent

The metal event object to be signaled or waited for.

let value: UInt64

The value to be signaled or waited for.

### Type Methods

static func signal(any MTLEvent, value: UInt64) -> RealityRenderer.MetalEventAction

Returns an action that represents signaling event with the value.

static func wait(for: any MTLEvent, value: UInt64) -> RealityRenderer.MetalEventAction

Returns an action that represents waiting for an event to reach the value.

## See Also

### Metal workflow rendering

class RealityRenderer

A renderer that displays a RealityKit scene in an existing Metal workflow.

struct CameraSettings

Settings for rendering with a camera.

struct CameraOutput

Output produced by rendering with a camera.

struct ImageBasedLight

Describe the lighting properties for the scene.

struct EntityCollection

A collection of entities in a RealityRenderer.

