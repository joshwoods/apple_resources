

- Combine
- Publishers
- Publishers.CombineLatest3
-  print(\_:to:) 

Instance Method

# print(\_:to:)

Prints log messages for all publishing events.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func print(
    _ prefix: String = "",
    to stream: (any TextOutputStream)? = nil
) -> Publishers.Print
```

## Parameters 

`prefix`  

A string —- which defaults to empty -— with which to prefix all log messages.

`stream`  

A stream for text output that receives messages, and which directs output to the console by default. A custom stream can be used to log messages to other destinations.

## Return Value

A publisher that prints log messages for all publishing events.

## Discussion

Use print(_:to:) to log messages the console.

In the example below, log messages are printed on the console:

```
let integers = (1...2)
cancellable = integers.publisher
   .print("Logged a message", to: nil)
   .sink { _ in }

// Prints:
//  Logged a message: receive subscription: (1..

## See Also

### Debugging

func breakpoint(receiveSubscription: ((any Subscription) -> Bool)?, receiveOutput: ((Self.Output) -> Bool)?, receiveCompletion: ((Subscribers.Completion&lt;Self.Failure>) -> Bool)?) -> Publishers.Breakpoint&lt;Self>

Raises a debugger signal when a provided closure needs to stop the process in the debugger.

func breakpointOnError() -> Publishers.Breakpoint&lt;Self>

Raises a debugger signal upon receiving a failure.

func handleEvents(receiveSubscription: ((any Subscription) -> Void)?, receiveOutput: ((Self.Output) -> Void)?, receiveCompletion: ((Subscribers.Completion&lt;Self.Failure>) -> Void)?, receiveCancel: (() -> Void)?, receiveRequest: ((Subscribers.Demand) -> Void)?) -> Publishers.HandleEvents&lt;Self>

Performs the specified closures when publisher events occur.

