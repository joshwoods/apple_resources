

- Swift
- AsyncThrowingStream
- AsyncThrowingStream.Continuation
-  yield(with:) 

Instance Method

# yield(with:)

Resume the task awaiting the next iteration point by having it return normally or throw, based on a given result.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@discardableResult
func yield(with result: sending Result) -> AsyncThrowingStream.Continuation.YieldResult where Failure == any Error
```

Available when `Failure` conforms to `Error`.

## Parameters 

`result`  

A result to yield from the continuation. In the `.success(_:)` case, this returns the associated value from the iterator’s `next()` method. If the result is the `failure(_:)` case, this call terminates the stream with the result’s error, by calling `finish(throwing:)`.

## Return Value

A `YieldResult` that indicates the success or failure of the yield operation.

## Discussion

If nothing is awaiting the next value and the result is success, this call attempts to buffer the result’s element.

If you call this method repeatedly, each call returns immediately, without blocking for any awaiting consumption from the iteration.

## See Also

### Producing Elements

func yield(sending Element) -> AsyncThrowingStream&lt;Element, Failure>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally from its suspension point with a given element.

func yield() -> AsyncThrowingStream&lt;Element, Failure>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally from its suspension point.

enum YieldResult

A type that indicates the result of yielding a value to a client, by way of the continuation.

