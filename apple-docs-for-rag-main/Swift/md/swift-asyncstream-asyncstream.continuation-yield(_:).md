

- Swift
- AsyncStream
- AsyncStream.Continuation
-  yield(\_:) 

Instance Method

# yield(\_:)

Resume the task awaiting the next iteration point by having it return normally from its suspension point with a given element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@discardableResult
func yield(_ value: sending Element) -> AsyncStream.Continuation.YieldResult
```

## Parameters 

`value`  

The value to yield from the continuation.

## Return Value

A `YieldResult` that indicates the success or failure of the yield operation.

## Discussion

If nothing is awaiting the next value, this method attempts to buffer the result’s element.

This can be called more than once and returns to the caller immediately without blocking for any awaiting consumption from the iteration.

## See Also

### Producing Elements

func yield(with: sending Result&lt;Element, Never>) -> AsyncStream&lt;Element>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally from its suspension point with a given result’s success value.

func yield() -> AsyncStream&lt;Element>.Continuation.YieldResult

Resume the task awaiting the next iteration point by having it return normally from its suspension point.

enum YieldResult

A type that indicates the result of yielding a value to a client, by way of the continuation.

