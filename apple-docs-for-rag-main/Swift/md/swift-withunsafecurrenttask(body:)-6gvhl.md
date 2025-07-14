

- Swift
-  withUnsafeCurrentTask(body:) 

Function

# withUnsafeCurrentTask(body:)

Calls a closure with an unsafe reference to the current task.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func withUnsafeCurrentTask(body: (UnsafeCurrentTask?) throws -> T) rethrows -> T
```

## Parameters 

`body`  

A closure that takes an `UnsafeCurrentTask` parameter. If `body` has a return value, that value is also used as the return value for the `withUnsafeCurrentTask(body:)` function.

## Return Value

The return value, if any, of the `body` closure.

## Discussion

If you call this function from the body of an asynchronous function, the unsafe task handle passed to the closure is always non-`nil` because an asynchronous function always runs in the context of a task. However, if you call this function from the body of a synchronous function, and that function isn’t executing in the context of any task, the unsafe task handle is `nil`.

Don’t store an unsafe task reference for use outside this method’s closure. Storing an unsafe reference doesn’t affect the task’s actual life cycle, and the behavior of accessing an unsafe task reference outside of the `withUnsafeCurrentTask(body:)` method’s closure isn’t defined. There’s no safe way to retrieve a reference to the current task and save it for long-term use. To query the current task without saving a reference to it, use properties like `currentPriority`. If you need to store a reference to a task, create an unstructured task using `Task.detached(priority:operation:)` instead.

## See Also

### Getting an Unsafe Reference to the Current Task

func withUnsafeCurrentTask&lt;T>(body: (UnsafeCurrentTask?) async throws -> T) async rethrows -> T

