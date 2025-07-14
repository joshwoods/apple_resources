

- Combine
- PassthroughSubject
-  send(subscription:) 

Instance Method

# send(subscription:)

Sends a subscription to the subscriber.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final func send(subscription: any Subscription)
```

## Parameters 

`subscription`  

The subscription instance through which the subscriber can request elements.

## Discussion

This call provides the Subject an opportunity to establish demand for any new upstream subscriptions.

## See Also

### Delivering Life Cycle Events to Subscribers

func send(completion: Subscribers.Completion&lt;Failure>)

Sends a completion signal to the subscriber.

