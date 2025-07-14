

- RealityKit
- RealityRenderer
- RealityRenderer.MetalEventAction
-  wait(for:value:) 

Type Method

# wait(for:value:)

Returns an action that represents waiting for an event to reach the value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
static func wait(
    for event: any MTLEvent,
    value: UInt64
) -> RealityRenderer.MetalEventAction
```

