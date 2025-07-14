

- Swift
- TaskGroup
-  spawnUnlessCancelled(priority:operation:) 

Instance Method

# spawnUnlessCancelled(priority:operation:)

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+Mac Catalyst 13.0+

``` source
mutating func spawnUnlessCancelled(
    priority: TaskPriority? = nil,
    operation: @escaping () async -> ChildTaskResult
) -> Bool
```

Available when `ChildTaskResult` conforms to `Sendable`.

## See Also

### Deprecated

func add(priority: TaskPriority?, operation: () async -> ChildTaskResult) async -> BoolDeprecated

func async(priority: TaskPriority?, operation: () async -> ChildTaskResult)Deprecated

func asyncUnlessCancelled(priority: TaskPriority?, operation: () async -> ChildTaskResult) -> BoolDeprecated

func spawn(priority: TaskPriority?, operation: () async -> ChildTaskResult)Deprecated

