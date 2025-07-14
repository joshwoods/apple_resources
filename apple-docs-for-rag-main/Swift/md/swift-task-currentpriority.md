

- Swift
- Task
-  currentPriority 

Type Property

# currentPriority

The current task’s priority.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static var currentPriority: TaskPriority { get }
```

Available when `Success` is `Never` and `Failure` is `Never`.

## Discussion

If you access this property outside of any task, this queries the system to determine the priority at which the current function is running. If the system can’t provide a priority, this property’s value is `Priority.default`.

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

static func detached(executorPreference: (any TaskExecutor)?, priority: TaskPriority?, operation: sending () async throws -> Success) -> Task&lt;Success, Failure>

Runs the given throwing operation asynchronously as part of a new top-level task.

static var basePriority: TaskPriority?

The current task’s base priority.

