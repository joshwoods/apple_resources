

- Combine
- Publishers
- Publishers.CombineLatest
-  receive(subscriber:) 

Instance Method

# receive(subscriber:)

Attaches the specified subscriber to this publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func receive(subscriber: S) where S : Subscriber, B.Failure == S.Failure, S.Input == (A.Output, B.Output)
```

## Parameters 

`subscriber`  

The subscriber to attach to this Publisher, after which it can receive values.

## Discussion

Implementations of Publisher must implement this method.

The provided implementation of subscribe(_:)calls this method.

## See Also

### Working with Subscribers

func subscribe&lt;S>(S)

Attaches the specified subscriber to this publisher.

func subscribe&lt;S>(S) -> AnyCancellable

Attaches the specified subject to this publisher.

