

- RealityKit
- ActionHandlerProtocol
-  actionUpdated(event:) 

Instance Method

# actionUpdated(event:)

The function used to respond to action updated events.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
mutating func actionUpdated(event: Self.EventType)
```

**Required** Default implementation provided.

## Discussion

An update event is raised after a start event, and the the animation time remains within the an action’s event interval.

## Default Implementations

### ActionHandlerProtocol Implementations

func actionUpdated(event: Self.EventType)

The function used to respond to action updated events.

