

- Swift
-  UnsafeThrowingContinuation Deprecated

Type Alias

# UnsafeThrowingContinuation

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 6.0+tvOS 13.0+

``` source
typealias UnsafeThrowingContinuation = UnsafeContinuation
```

Deprecated

please use UnsafeContinuation\

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

func withUnsafeThrowingContinuation&lt;T>(isolation: isolated (any Actor)?, (UnsafeContinuation&lt;T, any Error>) -> Void) async throws -> sending T

Invokes the passed in closure with a unsafe continuation for the current task.

