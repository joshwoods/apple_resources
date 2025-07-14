

- Swift
- Task
-  withCancellationHandler(handler:operation:) Deprecated

Type Method

# withCancellationHandler(handler:operation:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func withCancellationHandler(
    handler: () -> Void,
    operation: () async throws -> T
) async rethrows -> T
```

Available when `Success` is `Never` and `Failure` is `Never`.

Deprecated

\`Task.withCancellationHandler\` has been replaced by \`withTaskCancellationHandler\` and will be removed shortly.

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

static func runDetached(priority: TaskPriority?, operation: () async throws -> Success) -> Task&lt;Success, Failure>Deprecated

