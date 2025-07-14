

- Swift
- Task
-  detached(priority:operation:) 

Type Method

# detached(priority:operation:)

Runs the given nonthrowing operation asynchronously as part of a new top-level task.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@discardableResult
static func detached(
    priority: TaskPriority? = nil,
    operation: sending @escaping @isolated(any) () async -> Success
) -> Task
```

Available when `Success` conforms to `Sendable` and `Failure` is `Never`.

## Parameters 

`priority`  

The priority of the task.

`operation`  

The operation to perform.

## Return Value

A reference to the task.

## Discussion

Don’t use a detached task if it’s possible to model the operation using structured concurrency features like child tasks. Child tasks inherit the parent task’s priority and task-local storage, and canceling a parent task automatically cancels all of its child tasks. You need to handle these considerations manually with a detached task.

You need to keep a reference to the detached task if you want to cancel it by calling the `Task.cancel()` method. Discarding your reference to a detached task doesn’t implicitly cancel that task, it only makes it impossible for you to explicitly cancel the task.

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

