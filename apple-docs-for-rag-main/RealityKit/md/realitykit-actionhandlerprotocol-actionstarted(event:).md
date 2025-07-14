

- RealityKit
- ActionHandlerProtocol
-  actionStarted(event:) 

Instance Method

# actionStarted(event:)

The function used to respond to action started events.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
mutating func actionStarted(event: Self.EventType)
```

**Required** Default implementation provided.

## Discussion

A start event is raised when the animation time first falls within an event’s defined time interval.

## Default Implementations

### ActionHandlerProtocol Implementations

func actionStarted(event: Self.EventType)

The function used to respond to action started events.

