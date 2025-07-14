

- Swift
- ThrowingTaskGroup
-  async(priority:operation:) 

Instance Method

# async(priority:operation:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func async(
    priority: TaskPriority? = nil,
    operation: @escaping () async throws -> ChildTaskResult
)
```

Available when `ChildTaskResult` conforms to `Sendable` and `Failure` conforms to `Error`.

## See Also

### Deprecated

func add(priority: TaskPriority?, operation: () async throws -> ChildTaskResult) async -> BoolDeprecated

func asyncUnlessCancelled(priority: TaskPriority?, operation: () async throws -> ChildTaskResult) -> BoolDeprecated

func spawn(priority: TaskPriority?, operation: () async throws -> ChildTaskResult)Deprecated

func spawnUnlessCancelled(priority: TaskPriority?, operation: () async throws -> ChildTaskResult) -> BoolDeprecated

