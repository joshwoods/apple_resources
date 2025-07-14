

- Swift
- Task
-  detached(executorPreference:priority:operation:) 

Type Method

# detached(executorPreference:priority:operation:)

Runs the given throwing operation asynchronously as part of a new top-level task.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@discardableResult
static func detached(
    executorPreference taskExecutor: (any TaskExecutor)?,
    priority: TaskPriority? = nil,
    operation: sending @escaping () async throws -> Success
) -> Task
```

Available when `Success` conforms to `Sendable` and `Failure` is `any Error`.

## Parameters 

`taskExecutor`  

The preferred task executor for this task, and any child tasks created by it. Explicitly passing `nil` is interpreted as “no preference”.

`priority`  

The priority of the task. Pass `nil` to use the priority from `Task.currentPriority`.

`operation`  

The operation to perform.

## Return Value

A reference to the newly created task.

## Discussion

If the operation throws an error, this method propagates that error.

Don’t use a detached task if it’s possible to model the operation using structured concurrency features like child tasks. Child tasks inherit the parent task’s priority and task-local storage, and canceling a parent task automatically cancels all of its child tasks. You need to handle these considerations manually with a detached task.

You need to keep a reference to the detached task if you want to cancel it by calling the `Task.cancel()` method. Discarding your reference to a detached task doesn’t implicitly cancel that task, it only makes it impossible for you to explicitly cancel the task.

See Also

`withTaskExecutorPreference(_:operation:)`

## See Also

### Creating a Task

init(priority: TaskPriority?, operation: sending () async -> Success)

Runs the given nonthrowing operation asynchronously as part of a new top-level task on behalf of the current actor.

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

static var currentPriority: TaskPriority

The current task’s priority.

static var basePriority: TaskPriority?

The current task’s base priority.

