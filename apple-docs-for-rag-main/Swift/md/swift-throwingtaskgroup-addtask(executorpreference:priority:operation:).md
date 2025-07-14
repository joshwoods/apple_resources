

- Swift
- ThrowingTaskGroup
-  addTask(executorPreference:priority:operation:) 

Instance Method

# addTask(executorPreference:priority:operation:)

Adds a child task to the group and enqueue it on the specified executor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func addTask(
    executorPreference taskExecutor: (any TaskExecutor)?,
    priority: TaskPriority? = nil,
    operation: sending @escaping @isolated(any) () async throws -> ChildTaskResult
)
```

Available when `ChildTaskResult` conforms to `Sendable` and `Failure` conforms to `Error`.

## Parameters 

`taskExecutor`  

The task executor that the child task should be started on and keep using. If `nil` is passed explicitly, that parent task’s executor preference (if any), will be ignored. In order to inherit the parent task’s executor preference invoke `addTask()` without passing a value to the `taskExecutor` parameter, and it will be inherited automatically.

`priority`  

The priority of the operation task. Omit this parameter or pass `.unspecified` to set the child task’s priority to the priority of the group.

`operation`  

The operation to execute as part of the task group.

