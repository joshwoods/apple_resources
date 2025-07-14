

- RealityKit
- RealityRenderer
- RealityRenderer.MetalEventAction
-  signal(\_:value:) 

Type Method

# signal(\_:value:)

Returns an action that represents signaling event with the value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
static func signal(
    _ event: any MTLEvent,
    value: UInt64
) -> RealityRenderer.MetalEventAction
```

