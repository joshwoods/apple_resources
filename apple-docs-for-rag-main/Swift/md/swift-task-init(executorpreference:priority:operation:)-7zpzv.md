

- Swift
- Task
-  init(executorPreference:priority:operation:) 

Initializer

# init(executorPreference:priority:operation:)

Runs the given nonthrowing operation asynchronously as part of a new top-level task on behalf of the current actor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@discardableResult
init(
    executorPreference taskExecutor: consuming (any TaskExecutor)?,
    priority: TaskPriority? = nil,
    operation: sending @escaping () async -> Success
)
```

Available when `Success` conforms to `Sendable` and `Failure` is `Never`.

## Parameters 

`taskExecutor`  

The preferred task executor for this task, and any child tasks created by it. Explicitly passing `nil` is interpreted as “no preference”.

`priority`  

The priority of the task. Pass `nil` to use the priority from `Task.currentPriority`.

`operation`  

The operation to perform.

## Discussion

This overload allows specifying a preferred TaskExecutor on which the `operation`, as well as all child tasks created from this task will be executing whenever possible. Refer to TaskExecutor for a detailed discussion of the effect of task executors on execution semantics of asynchronous code.

Use this function when creating asynchronous work that operates on behalf of the synchronous function that calls it. Like `Task.detached(priority:operation:)`, this function creates a separate, top-level task. Unlike `Task.detached(priority:operation:)`, the task created by `Task.init(priority:operation:)` inherits the priority and actor context of the caller, so the operation is treated more like an asynchronous extension to the synchronous operation.

You need to keep a reference to the task if you want to cancel it by calling the `Task.cancel()` method. Discarding your reference to a detached task doesn’t implicitly cancel that task, it only makes it impossible for you to explicitly cancel the task.

See Also

`withTaskExecutorPreference(_:operation:)`

## See Also

### Creating a Task

init(priority: TaskPriority?, operation: sending () async -> Success)

Runs the given nonthrowing operation asynchronously as part of a new top-level task on behalf of the current actor.

init(priority: TaskPriority?, operation: sending () async throws -> Success)

Runs the given throwing operation asynchronously as part of a new top-level task on behalf of the current actor.

init(executorPreference: consuming (any TaskExecutor)?, priority: TaskPriority?, operation: sending () async throws -> Success)

Runs the given throwing operation asynchronously as part of a new top-level task on behalf of the current actor.

static func detached(priority: TaskPriority?, operation: sending () async -> Success) -> Task&lt;Success, Failure>

Runs the given nonthrowing operation asynchronously as part of a new top-level task.

static func detached(priority: TaskPriority?, operation: sending () async throws -> Success) -> Task&lt;Success, Failure>

Runs the given throwing operation asynchronously as part of a new top-level task.

static func detached(executorPreference: (any TaskExecutor)?, priority: TaskPriority?, operation: sending () async -> Success) -> Task&lt;Success, Failure>

Runs the given nonthrowing operation asynchronously as part of a new top-level task.

static func detached(executorPreference: (any TaskExecutor)?, priority: TaskPriority?, operation: sending () async throws -> Success) -> Task&lt;Success, Failure>

Runs the given throwing operation asynchronously as part of a new top-level task.

static var currentPriority: TaskPriority

The current task’s priority.

static var basePriority: TaskPriority?

The current task’s base priority.

