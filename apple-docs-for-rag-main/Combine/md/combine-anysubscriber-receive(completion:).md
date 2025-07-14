

- Combine
- AnySubscriber
-  receive(completion:) 

Instance Method

# receive(completion:)

Tells the subscriber that the publisher has completed publishing, either normally or with an error.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func receive(completion: Subscribers.Completion)
```

## Parameters 

`completion`  

A Subscribers.Completion case indicating whether publishing completed normally or with an error.

## See Also

### Receiving Life Cycle Events

func receive(subscription: any Subscription)

Tells the subscriber that it has successfully subscribed to the publisher and may request items.

