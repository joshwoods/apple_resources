

- Swift
- ThrowingDiscardingTaskGroup
-  addTask(priority:operation:) 

Instance Method

# addTask(priority:operation:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
mutating func addTask(
    priority: TaskPriority? = nil,
    operation: sending @escaping @isolated(any) () async throws -> Void
)
```

