

- RealityKit
- ActionHandlerProtocol
-  actionSkipped(event:) 

Instance Method

# actionSkipped(event:)

The function used to respond to action skipped events.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
mutating func actionSkipped(event: Self.EventType)
```

**Required** Default implementation provided.

## Discussion

The animation system can skip over an event interval due to scrubbing or choppy frame rate.

## Default Implementations

### ActionHandlerProtocol Implementations

func actionSkipped(event: Self.EventType)

The function used to respond to action skipped events.

