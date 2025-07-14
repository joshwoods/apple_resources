

- Swift
-  ThrowingDiscardingTaskGroup 

Structure

# ThrowingDiscardingTaskGroup

A throwing discarding group that contains dynamically created child tasks.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@frozen
struct ThrowingDiscardingTaskGroup where Failure : Error
```

## Overview

To create a discarding task group, call the `withDiscardingTaskGroup(returning:body:)` method.

Don’t use a task group from outside the task where you created it. In most cases, the Swift type system prevents a task group from escaping like that because adding a child task to a task group is a mutating operation, and mutation operations can’t be performed from a concurrent execution context like a child task.

### Task execution order

Tasks added to a task group execute concurrently, and may be scheduled in any order.

### Discarding behavior

A discarding task group eagerly discards and releases its child tasks as soon as they complete. This allows for the efficient releasing of memory used by those tasks, which are not retained for future `next()` calls, as would be the case with a TaskGroup.

### Cancellation behavior

A throwing discarding task group becomes cancelled in one of the following ways:

- when cancelAll() is invoked on it,

- when an error is thrown out of the `withThrowingDiscardingTaskGroup { ... }` closure,

- when the Task running this task group is cancelled.

But also, and uniquely in *discarding* task groups:

- when *any* of its child tasks throws.

The group becoming cancelled automatically, and cancelling all of its child tasks, whenever *any* child task throws an error is a behavior unique to discarding task groups, because achieving such semantics is not possible otherwise, due to the missing `next()` method on discarding groups. Accumulating task groups can implement this by manually polling `next()` and deciding to `cancelAll()` when they decide an error should cause the group to become cancelled, however a discarding group cannot poll child tasks for results and therefore assumes that child task throws are an indication of a group wide failure. In order to avoid such behavior, use a DiscardingTaskGroup instead of a throwing one, or catch specific errors in operations submitted using `addTask`.

Since a `ThrowingDiscardingTaskGroup` is a structured concurrency primitive, cancellation is automatically propagated through all of its child-tasks (and their child tasks).

A cancelled task group can still keep adding tasks, however they will start being immediately cancelled, and may act accordingly to this. To avoid adding new tasks to an already cancelled task group, use `addTaskUnlessCancelled(priority:body:)` rather than the plain `addTask(priority:body:)` which adds tasks unconditionally.

For information about the language-level concurrency model that `DiscardingTaskGroup` is part of, see Concurrency in The Swift Programming Language.

See Also

TaskGroup

See Also

ThrowingTaskGroup

See Also

DiscardingTaskGroup

## Topics

### Instance Properties

var isCancelled: Bool

A Boolean value that indicates whether the group was canceled.

var isEmpty: Bool

A Boolean value that indicates whether the group has any remaining tasks.

### Instance Methods

func addTask(executorPreference: (any TaskExecutor)?, priority: TaskPriority?, operation: sending () async throws -> Void)

Adds a child task to the group and set it up with the passed in task executor preference.

func addTask(priority: TaskPriority?, operation: sending () async throws -> Void)

func addTaskUnlessCancelled(executorPreference: (any TaskExecutor)?, priority: TaskPriority?, operation: sending () async throws -> Void) -> Bool

Adds a child task to the group and set it up with the passed in task executor preference, unless the group has been canceled.

func addTaskUnlessCancelled(priority: TaskPriority?, operation: sending () async throws -> Void) -> Bool

func cancelAll()

Cancel all of the remaining tasks in the group.

## Relationships

### Conforms To

- BitwiseCopyable

  Conforms when `Failure` conforms to `Error`.

- Copyable

  Conforms when `Failure` conforms to `Error`.

## See Also

### Tasks

struct Task

A unit of asynchronous work.

struct TaskGroup

A group that contains dynamically created child tasks.

func withTaskGroup&lt;ChildTaskResult, GroupResult>(of: ChildTaskResult.Type, returning: GroupResult.Type, isolation: isolated (any Actor)?, body: (inout TaskGroup&lt;ChildTaskResult>) async -> GroupResult) async -> GroupResult

Starts a new scope that can contain a dynamic number of child tasks.

struct ThrowingTaskGroup

A group that contains throwing, dynamically created child tasks.

func withThrowingTaskGroup&lt;ChildTaskResult, GroupResult>(of: ChildTaskResult.Type, returning: GroupResult.Type, isolation: isolated (any Actor)?, body: (inout ThrowingTaskGroup&lt;ChildTaskResult, any Error>) async throws -> GroupResult) async rethrows -> GroupResult

Starts a new scope that can contain a dynamic number of throwing child tasks.

struct TaskPriority

The priority of a task.

struct DiscardingTaskGroup

A discarding group that contains dynamically created child tasks.

func withDiscardingTaskGroup&lt;GroupResult>(returning: GroupResult.Type, isolation: isolated (any Actor)?, body: (inout DiscardingTaskGroup) async -> GroupResult) async -> GroupResult

Starts a new scope that can contain a dynamic number of child tasks.

func withThrowingDiscardingTaskGroup&lt;GroupResult>(returning: GroupResult.Type, isolation: isolated (any Actor)?, body: (inout ThrowingDiscardingTaskGroup&lt;any Error>) async throws -> GroupResult) async throws -> GroupResult

Starts a new scope that can contain a dynamic number of child tasks.

struct UnsafeCurrentTask

An unsafe reference to the current task.

