

- Swift
- TaskGroup
-  addTaskUnlessCancelled(priority:operation:) 

Instance Method

# addTaskUnlessCancelled(priority:operation:)

Adds a child task to the group, unless the group has been canceled.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func addTaskUnlessCancelled(
    priority: TaskPriority? = nil,
    operation: sending @escaping @isolated(any) () async -> ChildTaskResult
) -> Bool
```

## Parameters 

`priority`  

The priority of the operation task. Omit this parameter or pass `.unspecified` to set the child task’s priority to the priority of the group.

`operation`  

The operation to execute as part of the task group.

## Return Value

`true` if the child task was added to the group; otherwise `false`.

