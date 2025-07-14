

- RealityKit
- ActionHandlerProtocol
-  actionEnded(event:) 

Instance Method

# actionEnded(event:)

The function used to respond to action ended events.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
mutating func actionEnded(event: Self.EventType)
```

**Required** Default implementation provided.

## Discussion

Action ended is raised after a ‘started’ event has taken place, and the animation time exits the event interval, or when the animation is terminated before completion.

## Default Implementations

### ActionHandlerProtocol Implementations

func actionEnded(event: Self.EventType)

The function used to respond to action ended events.

