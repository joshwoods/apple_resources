

- Swift
- Task
-  init(priority:operation:) 

Initializer

# init(priority:operation:)

Runs the given nonthrowing operation asynchronously as part of a new top-level task on behalf of the current actor.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@discardableResult
init(
    priority: TaskPriority? = nil,
    operation: sending @escaping @isolated(any) () async -> Success
)
```

Available when `Success` conforms to `Sendable` and `Failure` is `Never`.

## Parameters 

`priority`  

The priority of the task. Pass `nil` to use the priority from `Task.currentPriority`.

`operation`  

The operation to perform.

## Discussion

Use this function when creating asynchronous work that operates on behalf of the synchronous function that calls it. Like `Task.detached(priority:operation:)`, this function creates a separate, top-level task. Unlike `Task.detached(priority:operation:)`, the task created by `Task.init(priority:operation:)` inherits the priority and actor context of the caller, so the operation is treated more like an asynchronous extension to the synchronous operation.

You need to keep a reference to the task if you want to cancel it by calling the `Task.cancel()` method. Discarding your reference to a detached task doesn’t implicitly cancel that task, it only makes it impossible for you to explicitly cancel the task.

## See Also

### Creating a Task

init(priority: TaskPriority?, operation: sending () async throws -> Success)

Runs the given throwing operation asynchronously as part of a new top-level task on behalf of the current actor.

init(executorPreference: consuming (any TaskExecutor)?, priority: TaskPriority?, operation: sending () async -> Success)

Runs the given nonthrowing operation asynchronously as part of a new top-level task on behalf of the current actor.

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

