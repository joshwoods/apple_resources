

- Swift
- Result
- Result.Publisher
-  receive(subscriber:) 

Instance Method

# receive(subscriber:)

Attaches the specified subscriber to this publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func receive(subscriber: S) where Success == S.Input, Failure == S.Failure, S : Subscriber
```

## Parameters 

`subscriber`  

The subscriber to attach to this Result.Publisher, after which it can receive values.

## Discussion

Implementations of Result.Publisher must implement this method.

The provided implementation of `Publisher/subscribe(_:)-4u8kn`calls this method.

