

- Swift
- Task
-  Task.Group Deprecated

Type Alias

# Task.Group

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 6.0+tvOS 13.0+

``` source
typealias Group = ThrowingTaskGroup where TaskResult : Sendable
```

Available when `Success` is `Never` and `Failure` is `Never`.

Deprecated

\`Task.Group\` was replaced by \`ThrowingTaskGroup\` and \`TaskGroup\` and will be removed shortly.

## See Also

### Deprecated

typealias HandleDeprecated

typealias PriorityDeprecated

static func CancellationError() -> CancellationErrorDeprecated

func getResult() async -> Result&lt;Success, Failure>Deprecated

func get() async throws -> SuccessDeprecated

static func sleep(UInt64) asyncDeprecated

static func suspend() asyncDeprecated

static func runDetached(priority: TaskPriority?, operation: () async throws -> Success) -> Task&lt;Success, Failure>Deprecated

static func withCancellationHandler&lt;T>(handler: () -> Void, operation: () async throws -> T) async rethrows -> TDeprecated

