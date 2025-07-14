

- Swift
- TaskGroup
-  add(priority:operation:) 

Instance Method

# add(priority:operation:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+visionOS 1.0+

``` source
mutating func add(
    priority: TaskPriority? = nil,
    operation: @escaping () async -> ChildTaskResult
) async -> Bool
```

Available when `ChildTaskResult` conforms to `Sendable`.

## See Also

### Deprecated

func async(priority: TaskPriority?, operation: () async -> ChildTaskResult)Deprecated

func asyncUnlessCancelled(priority: TaskPriority?, operation: () async -> ChildTaskResult) -> BoolDeprecated

func spawn(priority: TaskPriority?, operation: () async -> ChildTaskResult)Deprecated

func spawnUnlessCancelled(priority: TaskPriority?, operation: () async -> ChildTaskResult) -> BoolDeprecated

