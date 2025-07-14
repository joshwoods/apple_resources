

- Combine
- PassthroughSubject
-  send(completion:) 

Instance Method

# send(completion:)

Sends a completion signal to the subscriber.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final func send(completion: Subscribers.Completion)
```

## Parameters 

`completion`  

A `Completion` instance which indicates whether publishing has finished normally or failed with an error.

## See Also

### Delivering Life Cycle Events to Subscribers

func send(subscription: any Subscription)

Sends a subscription to the subscriber.

