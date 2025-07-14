

- Swift
- DiscardingTaskGroup
-  addTaskUnlessCancelled(priority:operation:) 

Instance Method

# addTaskUnlessCancelled(priority:operation:)

Adds a child task to the group, unless the group has been canceled.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
mutating func addTaskUnlessCancelled(
    priority: TaskPriority? = nil,
    operation: sending @escaping @isolated(any) () async -> Void
) -> Bool
```

## Parameters 

`priority`  

The priority of the operation task. Omit this parameter or pass `.unspecified` to set the child task’s priority to the priority of the group.

`operation`  

The operation to execute as part of the task group.

## Return Value

`true` if the child task was added to the group; otherwise `false`.

