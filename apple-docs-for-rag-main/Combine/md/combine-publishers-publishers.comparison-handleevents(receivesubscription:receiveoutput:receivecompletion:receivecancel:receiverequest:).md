

- Combine
- Publishers
- Publishers.Comparison
-  handleEvents(receiveSubscription:receiveOutput:receiveCompletion:receiveCancel:receiveRequest:) 

Instance Method

# handleEvents(receiveSubscription:receiveOutput:receiveCompletion:receiveCancel:receiveRequest:)

Performs the specified closures when publisher events occur.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func handleEvents(
    receiveSubscription: ((any Subscription) -> Void)? = nil,
    receiveOutput: ((Self.Output) -> Void)? = nil,
    receiveCompletion: ((Subscribers.Completion) -> Void)? = nil,
    receiveCancel: (() -> Void)? = nil,
    receiveRequest: ((Subscribers.Demand) -> Void)? = nil
) -> Publishers.HandleEvents
```

## Parameters 

`receiveSubscription`  

An optional closure that executes when the publisher receives the subscription from the upstream publisher. This value defaults to `nil`.

`receiveOutput`  

An optional closure that executes when the publisher receives a value from the upstream publisher. This value defaults to `nil`.

`receiveCompletion`  

An optional closure that executes when the upstream publisher finishes normally or terminates with an error. This value defaults to `nil`.

`receiveCancel`  

An optional closure that executes when the downstream receiver cancels publishing. This value defaults to `nil`.

`receiveRequest`  

An optional closure that executes when the publisher receives a request for more elements. This value defaults to `nil`.

## Return Value

A publisher that performs the specified closures when publisher events occur.

## Discussion

Use handleEvents(receiveSubscription:receiveOutput:receiveCompletion:receiveCancel:receiveRequest:) when you want to examine elements as they progress through the stages of the publisher’s lifecycle.

In the example below, a publisher of integers shows the effect of printing debugging information at each stage of the element-processing lifecycle:

```
let integers = (0...2)
cancellable = integers.publisher
    .handleEvents(receiveSubscription: { subs in
        print("Subscription: \(subs.combineIdentifier)")
    }, receiveOutput: { anInt in
        print("in output handler, received \(anInt)")
    }, receiveCompletion: { _ in
        print("in completion handler")
    }, receiveCancel: {
        print("received cancel")
    }, receiveRequest: { (demand) in
        print("received demand: \(demand.description)")
    })
    .sink { _ in return }

// Prints:
//   received demand: unlimited
//   Subscription: 0x7f81284734c0
//   in output handler, received 0
//   in output handler, received 1
//   in output handler, received 2
//   in completion handler
```

## See Also

### Debugging

func breakpoint(receiveSubscription: ((any Subscription) -> Bool)?, receiveOutput: ((Self.Output) -> Bool)?, receiveCompletion: ((Subscribers.Completion&lt;Self.Failure>) -> Bool)?) -> Publishers.Breakpoint&lt;Self>

Raises a debugger signal when a provided closure needs to stop the process in the debugger.

func breakpointOnError() -> Publishers.Breakpoint&lt;Self>

Raises a debugger signal upon receiving a failure.

func print(String, to: (any TextOutputStream)?) -> Publishers.Print&lt;Self>

Prints log messages for all publishing events.

