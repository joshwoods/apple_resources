

- Combine
- ConnectablePublisher
-  autoconnect() 

Instance Method

# autoconnect()

Automates the process of connecting or disconnecting from this connectable publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func autoconnect() -> Publishers.Autoconnect
```

## Return Value

A publisher which automatically connects to its upstream connectable publisher.

## Mentioned in 

Controlling Publishing with Connectable Publishers

Replacing Foundation Timers with Timer Publishers

## Discussion

Use autoconnect() to simplify working with ConnectablePublisher instances, such as Timer.TimerPublisher in the Foundation framework.

In the following example, the publish(every:tolerance:on:in:options:) operator creates a Timer.TimerPublisher, which is a ConnectablePublisher. As a result, subscribers don’t receive any values until after a call to connect(). For convenience when working with a single subscriber, the autoconnect() operator performs the connect() call when attached to by the subscriber.

```
cancellable = Timer.publish(every: 1, on: .main, in: .default)
    .autoconnect()
    .sink { date in
        print ("Date now: \(date)")
    }
```

