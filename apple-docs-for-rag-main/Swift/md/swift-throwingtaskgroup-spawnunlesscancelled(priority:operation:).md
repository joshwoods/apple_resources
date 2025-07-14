

- Swift
- ThrowingTaskGroup
-  spawnUnlessCancelled(priority:operation:) 

Instance Method

# spawnUnlessCancelled(priority:operation:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+visionOS 1.0+

``` source
mutating func spawnUnlessCancelled(
    priority: TaskPriority? = nil,
    operation: @escaping () async throws -> ChildTaskResult
) -> Bool
```

Available when `ChildTaskResult` conforms to `Sendable` and `Failure` conforms to `Error`.

## See Also

### Deprecated

func add(priority: TaskPriority?, operation: () async throws -> ChildTaskResult) async -> BoolDeprecated

func async(priority: TaskPriority?, operation: () async throws -> ChildTaskResult)Deprecated

func asyncUnlessCancelled(priority: TaskPriority?, operation: () async throws -> ChildTaskResult) -> BoolDeprecated

func spawn(priority: TaskPriority?, operation: () async throws -> ChildTaskResult)Deprecated

