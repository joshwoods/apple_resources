

- RealityKit
- ActionHandlerProtocol
-  actionResumed(event:) 

Instance Method

# actionResumed(event:)

The function used to respond to action resumed events.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
mutating func actionResumed(event: Self.EventType)
```

**Required** Default implementation provided.

## Discussion

Action resumed is raised when animation playback is resumed after being paused.

## Default Implementations

### ActionHandlerProtocol Implementations

func actionResumed(event: Self.EventType)

The function used to respond to action resumed events. Action resumed is raised when animation playback is resumed after being paused.

