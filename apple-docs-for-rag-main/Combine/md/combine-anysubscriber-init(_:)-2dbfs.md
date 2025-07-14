

- Combine
- AnySubscriber
-  init(\_:) 

Initializer

# init(\_:)

Creates a type-erasing subscriber to wrap an existing subscriber.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(_ s: S) where Input == S.Input, Failure == S.Failure, S : Subscriber
```

## Parameters 

`s`  

The subscriber to type-erase.

## See Also

### Creating a Type-Erased Subscriber

init(receiveSubscription: ((any Subscription) -> Void)?, receiveValue: ((Input) -> Subscribers.Demand)?, receiveCompletion: ((Subscribers.Completion&lt;Failure>) -> Void)?)

Creates a type-erasing subscriber that executes the provided closures.

