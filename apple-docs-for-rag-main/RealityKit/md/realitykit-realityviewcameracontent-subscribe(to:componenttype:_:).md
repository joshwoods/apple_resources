

- RealityKit
- RealityViewCameraContent
-  subscribe(to:componentType:\_:) 

Instance Method

# subscribe(to:componentType:\_:)

Subscribes to an event type, optionally limited to a specific component type for component events.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
func subscribe(
    to event: E.Type,
    componentType: (any Component.Type)? = nil,
    _ handler: @escaping (E) -> Void
) -> EventSubscription where E : Event
```

## Parameters 

`event`  

The event type to subscribe to. For example, SceneEvents.Update or ComponentEvents.DidActivate.

`componentType`  

An optional component type to filter events to if the event is of the type ComponentEvents. Set to `nil` to listen for all events of the event type within the view content.

`handler`  

A closure that runs when the `event` occurs.

## Return Value

An object that represents the subscription to this event stream.

## Discussion

Events you can subscribe to including scene updates, SceneEvents.Update, or when an animation ends, AnimationEvents.PlaybackCompleted.

