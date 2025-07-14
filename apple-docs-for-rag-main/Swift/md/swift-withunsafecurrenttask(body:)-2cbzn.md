

- Swift
-  withUnsafeCurrentTask(body:) 

Function

# withUnsafeCurrentTask(body:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func withUnsafeCurrentTask(body: (UnsafeCurrentTask?) async throws -> T) async rethrows -> T
```

## See Also

### Getting an Unsafe Reference to the Current Task

func withUnsafeCurrentTask&lt;T>(body: (UnsafeCurrentTask?) throws -> T) rethrows -> T

Calls a closure with an unsafe reference to the current task.

