

- Swift
- ThrowingTaskGroup
-  add(priority:operation:) 

Instance Method

# add(priority:operation:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 6.0+tvOS 13.0+

``` source
mutating func add(
    priority: TaskPriority? = nil,
    operation: @escaping () async throws -> ChildTaskResult
) async -> Bool
```

Available when `ChildTaskResult` conforms to `Sendable` and `Failure` conforms to `Error`.

## See Also

### Deprecated

func async(priority: TaskPriority?, operation: () async throws -> ChildTaskResult)Deprecated

func asyncUnlessCancelled(priority: TaskPriority?, operation: () async throws -> ChildTaskResult) -> BoolDeprecated

func spawn(priority: TaskPriority?, operation: () async throws -> ChildTaskResult)Deprecated

func spawnUnlessCancelled(priority: TaskPriority?, operation: () async throws -> ChildTaskResult) -> BoolDeprecated

