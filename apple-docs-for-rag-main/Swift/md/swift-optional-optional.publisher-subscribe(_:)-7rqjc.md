

- Swift
- Optional
- Optional.Publisher
-  subscribe(\_:) 

Instance Method

# subscribe(\_:)

Attaches the specified subscriber to this publisher.

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func subscribe(_ subscriber: S) where S : Subscriber, Self.Failure == S.Failure, Self.Output == S.Input
```

## Parameters 

`subscriber`  

The subscriber to attach to this publisher. After attaching, the subscriber can start to receive values.

## Discussion

Always call this function instead of receive(subscriber:). Adopters of Optional.Publisher must implement receive(subscriber:). The implementation of `Publisher/subscribe(_:)-4u8kn` provided by Optional.Publisher calls through to receive(subscriber:).

