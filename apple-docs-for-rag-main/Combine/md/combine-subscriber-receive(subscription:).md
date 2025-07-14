

- Combine
- Subscriber
-  receive(subscription:) 

Instance Method

# receive(subscription:)

Tells the subscriber that it has successfully subscribed to the publisher and may request items.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func receive(subscription: any Subscription)
```

**Required**

## Parameters 

`subscription`  

A subscription that represents the connection between publisher and subscriber.

## Discussion

Use the received Subscription to request items from the publisher.

## See Also

### Receiving Life Cycle Events

func receive(completion: Subscribers.Completion&lt;Self.Failure>)

Tells the subscriber that the publisher has completed publishing, either normally or with an error.

**Required**

enum Completion

A signal that a publisher doesn’t produce additional elements, either due to normal completion or an error.

