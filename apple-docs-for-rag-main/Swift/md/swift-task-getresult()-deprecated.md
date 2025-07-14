

- Swift
- Task
-  getResult() Deprecated

Instance Method

# getResult()

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func getResult() async -> Result
```

Available when `Success` conforms to `Sendable` and `Failure` conforms to `Error`.

Deprecated

getResult() has been replaced by .result

## See Also

### Deprecated

typealias GroupDeprecated

typealias HandleDeprecated

typealias PriorityDeprecated

static func CancellationError() -> CancellationErrorDeprecated

func get() async throws -> SuccessDeprecated

static func sleep(UInt64) asyncDeprecated

static func suspend() asyncDeprecated

static func runDetached(priority: TaskPriority?, operation: () async throws -> Success) -> Task&lt;Success, Failure>Deprecated

static func withCancellationHandler&lt;T>(handler: () -> Void, operation: () async throws -> T) async rethrows -> TDeprecated

