

- Swift
- Task
-  runDetached(priority:operation:) Deprecated

Type Method

# runDetached(priority:operation:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 6.0+tvOS 13.0+

``` source
@discardableResult
static func runDetached(
    priority: TaskPriority? = nil,
    operation: @escaping () async throws -> Success
) -> Task
```

Available when `Success` conforms to `Sendable` and `Failure` is `any Error`.

Deprecated

\`Task.runDetached\` was replaced by \`Task.detached\` and will be removed shortly.

## See Also

### Deprecated

typealias GroupDeprecated

typealias HandleDeprecated

typealias PriorityDeprecated

static func CancellationError() -> CancellationErrorDeprecated

func getResult() async -> Result&lt;Success, Failure>Deprecated

func get() async throws -> SuccessDeprecated

static func sleep(UInt64) asyncDeprecated

static func suspend() asyncDeprecated

static func withCancellationHandler&lt;T>(handler: () -> Void, operation: () async throws -> T) async rethrows -> TDeprecated

