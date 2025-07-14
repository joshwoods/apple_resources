

- RealityKit
- ActionHandlerProtocol
-  actionTerminated(event:) 

Instance Method

# actionTerminated(event:)

The function used to respond to action terminated events.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
mutating func actionTerminated(event: Self.EventType)
```

**Required** Default implementation provided.

## Discussion

Action terminated is raised when playback is terminated and the animation is removed from the animation system. This can occur before the animation has a chance to complete if the user manually stops the animation by calling stop().

## Default Implementations

### ActionHandlerProtocol Implementations

func actionTerminated(event: Self.EventType)

The function used to respond to action terminated events.

