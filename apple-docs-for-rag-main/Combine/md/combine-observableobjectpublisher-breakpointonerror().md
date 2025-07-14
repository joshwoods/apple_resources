

- Combine
- ObservableObjectPublisher
-  breakpointOnError() 

Instance Method

# breakpointOnError()

Raises a debugger signal upon receiving a failure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func breakpointOnError() -> Publishers.Breakpoint
```

## Return Value

A publisher that raises a debugger signal upon receiving a failure.

## Discussion

When the upstream publisher fails with an error, this publisher raises the `SIGTRAP` signal, which stops the process in the debugger. Otherwise, this publisher passes through values and completions as-is.

In this example a PassthroughSubject publishes strings, but its downstream tryMap(_:) operator throws an error. This sends the error downstream as a Subscribers.Completion.failure(_:). The breakpointOnError() operator receives this completion and stops the app in the debugger.

```
 struct CustomError : Error {}
 let publisher = PassthroughSubject()
 cancellable = publisher
     .tryMap { stringValue in
         throw CustomError()
     }
     .breakpointOnError()
     .sink(
         receiveCompletion: { completion in print("Completion: \(String(describing: completion))") },
         receiveValue: { aValue in print("Result: \(String(describing: aValue))") }
     )

 publisher.send("TEST DATA")

 // Prints: "error: Execution was interrupted, reason: signal SIGTRAP."
 // Depending on your specific environment, the console messages may
 // also include stack trace information, which is not shown here.
```

## See Also

### Debugging

func breakpoint(receiveSubscription: ((any Subscription) -> Bool)?, receiveOutput: ((Self.Output) -> Bool)?, receiveCompletion: ((Subscribers.Completion&lt;Self.Failure>) -> Bool)?) -> Publishers.Breakpoint&lt;Self>

Raises a debugger signal when a provided closure needs to stop the process in the debugger.

func handleEvents(receiveSubscription: ((any Subscription) -> Void)?, receiveOutput: ((Self.Output) -> Void)?, receiveCompletion: ((Subscribers.Completion&lt;Self.Failure>) -> Void)?, receiveCancel: (() -> Void)?, receiveRequest: ((Subscribers.Demand) -> Void)?) -> Publishers.HandleEvents&lt;Self>

Performs the specified closures when publisher events occur.

func print(String, to: (any TextOutputStream)?) -> Publishers.Print&lt;Self>

Prints log messages for all publishing events.

