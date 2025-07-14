

- Combine
- AnySubscriber
-  init(receiveSubscription:receiveValue:receiveCompletion:) 

Initializer

# init(receiveSubscription:receiveValue:receiveCompletion:)

Creates a type-erasing subscriber that executes the provided closures.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    receiveSubscription: ((any Subscription) -> Void)? = nil,
    receiveValue: ((Input) -> Subscribers.Demand)? = nil,
    receiveCompletion: ((Subscribers.Completion) -> Void)? = nil
)
```

## Parameters 

`receiveSubscription`  

A closure to execute when the subscriber receives the initial subscription from the publisher.

`receiveValue`  

A closure to execute when the subscriber receives a value from the publisher.

`receiveCompletion`  

A closure to execute when the subscriber receives a completion callback from the publisher.

## See Also

### Creating a Type-Erased Subscriber

init&lt;S>(S)

Creates a type-erasing subscriber to wrap an existing subscriber.

