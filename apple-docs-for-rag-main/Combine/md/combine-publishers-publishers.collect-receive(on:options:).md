

- Combine
- Publishers
- Publishers.Collect
-  receive(on:options:) 

Instance Method

# receive(on:options:)

Specifies the scheduler on which to receive elements from the publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func receive(
    on scheduler: S,
    options: S.SchedulerOptions? = nil
) -> Publishers.ReceiveOn where S : Scheduler
```

## Parameters 

`scheduler`  

The scheduler the publisher uses for element delivery.

`options`  

Scheduler options used to customize element delivery.

## Return Value

A publisher that delivers elements using the specified scheduler.

## Discussion

You use the receive(on:options:) operator to receive results and completion on a specific scheduler, such as performing UI work on the main run loop. In contrast with subscribe(on:options:), which affects upstream messages, receive(on:options:) changes the execution context of downstream messages.

In the following example, the subscribe(on:options:) operator causes `jsonPublisher` to receive requests on `backgroundQueue`, while the receive(on:options:) causes `labelUpdater` to receive elements and completion on `RunLoop.main`.

```
let jsonPublisher = MyJSONLoaderPublisher() // Some publisher.
let labelUpdater = MyLabelUpdateSubscriber() // Some subscriber that updates the UI.

jsonPublisher
    .subscribe(on: backgroundQueue)
    .receive(on: RunLoop.main)
    .subscribe(labelUpdater)
```

Prefer receive(on:options:) over explicit use of dispatch queues when performing work in subscribers. For example, instead of the following pattern:

```
pub.sink {
    DispatchQueue.main.async {
        // Do something.
    }
}
```

Use this pattern instead:

```
pub.receive(on: DispatchQueue.main).sink {
    // Do something.
}
```

Note

receive(on:options:) doesn’t affect the scheduler used to call the subscriber’s receive(subscription:) method.

## See Also

### Specifying Schedulers

func subscribe&lt;S>(on: S, options: S.SchedulerOptions?) -> Publishers.SubscribeOn&lt;Self, S>

Specifies the scheduler on which to perform subscribe, cancel, and request operations.

