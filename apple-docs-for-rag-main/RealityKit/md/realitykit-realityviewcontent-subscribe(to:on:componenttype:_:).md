

- RealityKit
- RealityViewContent
-  subscribe(to:on:componentType:\_:) 

Instance Method

# subscribe(to:on:componentType:\_:)

Subscribes to an event type, optionally limited to events affecting a source entity or scene, or a specific component type for component events.

RealityKitSwiftUIvisionOS 1.0+

``` source
func subscribe(
    to event: E.Type,
    on sourceObject: (any EventSource)?,
    componentType: (any Component.Type)?,
    _ handler: @escaping (E) -> Void
) -> EventSubscription where E : Event
```

## Parameters 

`event`  

The event type to subscribe to. For example, SceneEvents.Update or ComponentEvents.DidActivate.

`sourceObject`  

An optional source for the event, such as an entity or a scene. Set to `nil` to listen for all events of the event type within the RealityViewContent.

`componentType`  

An optional component type to filter events to if the event is of the type ComponentEvents. Set to `nil` to listen for all events of the event type within the RealityViewContent.

`handler`  

A closure that runs when the `event` occurs.

## Return Value

An object that represents the subscription to this event stream.

