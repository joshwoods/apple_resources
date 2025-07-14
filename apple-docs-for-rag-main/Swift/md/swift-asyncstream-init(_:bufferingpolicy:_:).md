

- Swift
- AsyncStream
-  init(\_:bufferingPolicy:\_:) 

Initializer

# init(\_:bufferingPolicy:\_:)

Constructs an asynchronous stream for an element type, using the specified buffering policy and element-producing closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    _ elementType: Element.Type = Element.self,
    bufferingPolicy limit: AsyncStream.Continuation.BufferingPolicy = .unbounded,
    _ build: (AsyncStream.Continuation) -> Void
)
```

## Parameters 

`elementType`  

The type of element the `AsyncStream` produces.

`limit`  

A `Continuation.BufferingPolicy` value to set the stream’s buffering behavior. By default, the stream buffers an unlimited number of elements. You can also set the policy to buffer a specified number of oldest or newest elements.

`build`  

A custom closure that yields values to the `AsyncStream`. This closure receives an `AsyncStream.Continuation` instance that it uses to provide elements to the stream and terminate the stream when finished.

## Discussion

The `AsyncStream.Continuation` received by the `build` closure is appropriate for use in concurrent contexts. It is thread safe to send and finish; all calls to the continuation are serialized. However, calling this from multiple concurrent contexts could result in out-of-order delivery.

The following example shows an `AsyncStream` created with this initializer that produces 100 random numbers on a one-second interval, calling `yield(_:)` to deliver each element to the awaiting call point. When the `for` loop exits, the stream finishes by calling the continuation’s `finish()` method.

```
let stream = AsyncStream(Int.self,
                              bufferingPolicy: .bufferingNewest(5)) { continuation in
    Task.detached {
        for _ in 0..

## See Also

### Creating a Continuation-Based Stream

enum BufferingPolicy

A strategy that handles exhaustion of a buffer’s capacity.

struct Continuation

A mechanism to interface between synchronous code and an asynchronous stream.

