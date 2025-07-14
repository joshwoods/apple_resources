

- Swift
- ThrowingTaskGroup
-  addTaskUnlessCancelled(executorPreference:priority:operation:) 

Instance Method

# addTaskUnlessCancelled(executorPreference:priority:operation:)

Adds a child task to the group and enqueue it on the specified executor, unless the group has been canceled.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func addTaskUnlessCancelled(
    executorPreference taskExecutor: (any TaskExecutor)?,
    priority: TaskPriority? = nil,
    operation: sending @escaping @isolated(any) () async throws -> ChildTaskResult
) -> Bool
```

Available when `ChildTaskResult` conforms to `Sendable` and `Failure` conforms to `Error`.

## Parameters 

`taskExecutor`  

The task executor that the child task should be started on and keep using.

`priority`  

The priority of the operation task. Omit this parameter or pass `.unspecified` to set the child task’s priority to the priority of the group.

`operation`  

The operation to execute as part of the task group.

## Return Value

`true` if the child task was added to the group; otherwise `false`.

