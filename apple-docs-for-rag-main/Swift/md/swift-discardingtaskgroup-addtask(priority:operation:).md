

- Swift
- DiscardingTaskGroup
-  addTask(priority:operation:) 

Instance Method

# addTask(priority:operation:)

Adds a child task to the group.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
mutating func addTask(
    priority: TaskPriority? = nil,
    operation: sending @escaping @isolated(any) () async -> Void
)
```

## Parameters 

`priority`  

The priority of the operation task. Omit this parameter or pass `.unspecified` to set the child task’s priority to the priority of the group.

`operation`  

The operation to execute as part of the task group.

