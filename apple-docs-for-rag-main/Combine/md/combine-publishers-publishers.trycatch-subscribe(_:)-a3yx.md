

- Combine
- Publishers
- Publishers.TryCatch
-  subscribe(\_:) 

Instance Method

# subscribe(\_:)

Attaches the specified subscriber to this publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func subscribe(_ subscriber: S) where S : Subscriber, Self.Failure == S.Failure, Self.Output == S.Input
```

## Parameters 

`subscriber`  

The subscriber to attach to this publisher. After attaching, the subscriber can start to receive values.

## Discussion

Always call this function instead of receive(subscriber:). Adopters of Publisher must implement receive(subscriber:). The implementation of subscribe(_:) provided by Publisher calls through to receive(subscriber:).

## See Also

### Working with Subscribers

func receive&lt;S>(subscriber: S)

Attaches the specified subscriber to this publisher.

func subscribe&lt;S>(S) -> AnyCancellable

Attaches the specified subject to this publisher.

