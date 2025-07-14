

- Combine
- Publishers
- Publishers.TryReduce
-  subscribe(on:options:) 

Instance Method

# subscribe(on:options:)

Specifies the scheduler on which to perform subscribe, cancel, and request operations.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func subscribe(
    on scheduler: S,
    options: S.SchedulerOptions? = nil
) -> Publishers.SubscribeOn where S : Scheduler
```

## Parameters 

`scheduler`  

The scheduler used to send messages to upstream publishers.

`options`  

Options that customize the delivery of elements.

## Return Value

A publisher which performs upstream operations on the specified scheduler.

## Discussion

In contrast with receive(on:options:), which affects downstream messages, subscribe(on:options:) changes the execution context of upstream messages.

In the following example, the subscribe(on:options:) operator causes `ioPerformingPublisher` to receive requests on `backgroundQueue`, while the receive(on:options:) causes `uiUpdatingSubscriber` to receive elements and completion on `RunLoop.main`.

```
let ioPerformingPublisher == // Some publisher.
let uiUpdatingSubscriber == // Some subscriber that updates the UI.

ioPerformingPublisher
    .subscribe(on: backgroundQueue)
    .receive(on: RunLoop.main)
    .subscribe(uiUpdatingSubscriber)
```

Using subscribe(on:options:) also causes the upstream publisher to perform cancel() using the specfied scheduler.

## See Also

### Specifying Schedulers

func receive&lt;S>(on: S, options: S.SchedulerOptions?) -> Publishers.ReceiveOn&lt;Self, S>

Specifies the scheduler on which to receive elements from the publisher.

