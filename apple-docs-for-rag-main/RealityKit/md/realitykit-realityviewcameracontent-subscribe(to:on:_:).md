

- RealityKit
- RealityViewCameraContent
-  subscribe(to:on:\_:) 

Instance Method

# subscribe(to:on:\_:)

Subscribes to an event type, optionally limited to events affecting a source entity or scene.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
func subscribe(
    to event: E.Type,
    on sourceObject: (any EventSource)?,
    _ handler: @escaping (E) -> Void
) -> EventSubscription where E : Event
```

## Parameters 

`event`  

The event type to subscribe to. For example, SceneEvents.Update or ComponentEvents.DidActivate.

`sourceObject`  

An optional source for the event, such as an entity or a scene. Set to `nil` to listen for all events of the event type within the view content.

`handler`  

A closure that runs when the `event` occurs.

## Return Value

An object that represents the subscription to this event stream.

