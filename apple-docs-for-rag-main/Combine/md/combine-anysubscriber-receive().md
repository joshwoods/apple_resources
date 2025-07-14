

- Combine
- AnySubscriber
-  receive() 

Instance Method

# receive()

Tells the subscriber that a publisher of void elements is ready to receive further requests.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func receive() -> Subscribers.Demand
```

Available when `Input` is `()`.

## Return Value

A Subscribers.Demand instance indicating how many more elements the subscriber expects to receive.

## Discussion

Use `Void` inputs and outputs when you want to signal that an event has occurred, but don’t need to send the event itself.

## See Also

### Receiving Elements

func receive(Input) -> Subscribers.Demand

Tells the subscriber that the publisher has produced an element.

