

- Swift
- Task
-  Task.Priority Deprecated

Type Alias

# Task.Priority

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+visionOS 1.0+

``` source
typealias Priority = TaskPriority
```

Available when `Success` is `Never` and `Failure` is `Never`.

Deprecated

Task.Priority has been removed; use TaskPriority

## See Also

### Deprecated

typealias GroupDeprecated

typealias HandleDeprecated

static func CancellationError() -> CancellationErrorDeprecated

func getResult() async -> Result&lt;Success, Failure>Deprecated

func get() async throws -> SuccessDeprecated

static func sleep(UInt64) asyncDeprecated

static func suspend() asyncDeprecated

static func runDetached(priority: TaskPriority?, operation: () async throws -> Success) -> Task&lt;Success, Failure>Deprecated

static func withCancellationHandler&lt;T>(handler: () -> Void, operation: () async throws -> T) async rethrows -> TDeprecated

