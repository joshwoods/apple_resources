

- Swift
- AsyncStream
- AsyncStream.Continuation
-  yield() 

Instance Method

# yield()

Resume the task awaiting the next iteration point by having it return normally from its suspension point.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@discardableResult
func yield() -> AsyncStream.Continuation.YieldResult where Element == ()
```

## Return Value

A `YieldResult` that indicates the success or failure of the yield operation.

## Discussion

Use this method with `AsyncStream` instances whose `Element` type is `Void`. In this case, the `yield()` call unblocks the awaiting iteration; there is no value to return.

If you call this method repeatedly, each call returns immediately, without blocking for any awaiting consumption from the iteration.

## See Also

### Producing Elements

func yield(sending Element) -> AsyncStream&lt;Element>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally from its suspension point with a given element.

func yield(with: sending Result&lt;Element, Never>) -> AsyncStream&lt;Element>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally from its suspension point with a given result’s success value.

enum YieldResult

A type that indicates the result of yielding a value to a client, by way of the continuation.

