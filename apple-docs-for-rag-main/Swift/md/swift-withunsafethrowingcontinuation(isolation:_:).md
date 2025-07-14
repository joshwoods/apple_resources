

- Swift
-  withUnsafeThrowingContinuation(isolation:\_:) 

Function

# withUnsafeThrowingContinuation(isolation:\_:)

Invokes the passed in closure with a unsafe continuation for the current task.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func withUnsafeThrowingContinuation(
    isolation: isolated (any Actor)? = #isolation,
    _ fn: (UnsafeContinuation) -> Void
) async throws -> sending T
```

## Parameters 

`fn`  

A closure that takes an `UnsafeContinuation` parameter.

## Return Value

The value continuation is resumed with.

## Discussion

The body of the closure executes synchronously on the calling task, and once it returns the calling task is suspended. It is possible to immediately resume the task, or escape the continuation in order to complete it afterwards, which will then resume the suspended task.

If `resume(throwing:)` is called on the continuation, this function throws that error.

You must invoke the continuation’s `resume` method exactly once.

Missing to invoke it (eventually) will cause the calling task to remain suspended indefinitely which will result in the task “hanging” as well as being leaked with no possibility to destroy it.

Unlike the “checked” continuation variant, the `UnsafeContinuation` does not detect or diagnose any kind of misuse, so you need to be extra careful to avoid calling `resume` twice or forgetting to call resume before letting go of the continuation object.

See Also

`withUnsafeContinuation(function:_:)`

See Also

`withCheckedContinuation(function:_:)`

See Also

`withCheckedThrowingContinuation(function:_:)`

## See Also

### Continuations

struct CheckedContinuation

A mechanism to interface between synchronous and asynchronous code, logging correctness violations.

func withCheckedContinuation&lt;T>(isolation: isolated (any Actor)?, function: String, (CheckedContinuation&lt;T, Never>) -> Void) async -> sending T

Invokes the passed in closure with a checked continuation for the current task.

func withCheckedThrowingContinuation&lt;T>(isolation: isolated (any Actor)?, function: String, (CheckedContinuation&lt;T, any Error>) -> Void) async throws -> sending T

Invokes the passed in closure with a checked continuation for the current task.

struct UnsafeContinuation

A mechanism to interface between synchronous and asynchronous code, without correctness checking.

func withUnsafeContinuation&lt;T>(isolation: isolated (any Actor)?, (UnsafeContinuation&lt;T, Never>) -> Void) async -> sending T

Invokes the passed in closure with a unsafe continuation for the current task.

typealias UnsafeThrowingContinuationDeprecated

