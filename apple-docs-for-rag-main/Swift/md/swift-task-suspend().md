

- Swift
- Task
-  suspend() 

Type Method

# suspend()

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func suspend() async
```

Available when `Success` is `Never` and `Failure` is `Never`.

## See Also

### Deprecated

typealias GroupDeprecated

typealias HandleDeprecated

typealias PriorityDeprecated

static func CancellationError() -> CancellationErrorDeprecated

func getResult() async -> Result&lt;Success, Failure>Deprecated

func get() async throws -> SuccessDeprecated

static func sleep(UInt64) asyncDeprecated

static func runDetached(priority: TaskPriority?, operation: () async throws -> Success) -> Task&lt;Success, Failure>Deprecated

static func withCancellationHandler&lt;T>(handler: () -> Void, operation: () async throws -> T) async rethrows -> TDeprecated

