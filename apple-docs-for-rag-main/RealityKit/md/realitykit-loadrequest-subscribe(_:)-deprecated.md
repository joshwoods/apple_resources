

- RealityKit
- LoadRequest
-  subscribe(\_:) Deprecated

Instance Method

# subscribe(\_:)

Attaches the specified subscriber to this publisher.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 10.15–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func subscribe(_ subscriber: S) where Output == S.Input, S : Subscriber, S.Failure == any Error
```

## Parameters 

`subscriber`  

The subscriber to attach to this publisher. After attaching, the subscriber can start to receive values.

## Discussion

Always call this function instead of `Publisher/receive(subscriber:)`. Adopters of `Publisher` must implement `Publisher/receive(subscriber:)`. The implementation of `Publisher/subscribe(_:)-4u8kn` provided by `Publisher` calls through to `Publisher/receive(subscriber:)`.

## See Also

### Working with subscribers

func receive&lt;S>(subscriber: S)

Attaches the specified subscriber to this publisher.

Deprecated

func subscribe&lt;S>(S)

Attaches the specified subscriber to this publisher.

func subscribe&lt;S>(S) -> AnyCancellable

Attaches the specified subject to this publisher.

