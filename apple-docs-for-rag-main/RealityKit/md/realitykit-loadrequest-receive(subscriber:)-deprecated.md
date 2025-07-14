

- RealityKit
- LoadRequest
-  receive(subscriber:) Deprecated

Instance Method

# receive(subscriber:)

Attaches the specified subscriber to this publisher.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 10.15–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func receive(subscriber: S) where Output == S.Input, S : Subscriber, S.Failure == any Error
```

## Parameters 

`subscriber`  

The subscriber to attach to this `Publisher`, after which it can receive values.

## Discussion

Implementations of `Publisher` must implement this method.

The provided implementation of `Publisher/subscribe(_:)-4u8kn`calls this method.

## See Also

### Working with subscribers

func subscribe&lt;S>(S)

Attaches the specified subscriber to this publisher.

Deprecated

func subscribe&lt;S>(S)

Attaches the specified subscriber to this publisher.

func subscribe&lt;S>(S) -> AnyCancellable

Attaches the specified subject to this publisher.

