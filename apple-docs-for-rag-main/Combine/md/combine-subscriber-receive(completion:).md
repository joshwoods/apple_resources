

- Combine
- Subscriber
-  receive(completion:) 

Instance Method

# receive(completion:)

Tells the subscriber that the publisher has completed publishing, either normally or with an error.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func receive(completion: Subscribers.Completion)
```

**Required**

## Parameters 

`completion`  

A Subscribers.Completion case indicating whether publishing completed normally or with an error.

## See Also

### Receiving Life Cycle Events

func receive(subscription: any Subscription)

Tells the subscriber that it has successfully subscribed to the publisher and may request items.

**Required**

enum Completion

A signal that a publisher doesn’t produce additional elements, either due to normal completion or an error.

