

- Swift
- DiscardingTaskGroup
-  addTaskUnlessCancelled(operation:) 

Instance Method

# addTaskUnlessCancelled(operation:)

Adds a child task to the group, unless the group has been canceled.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
mutating func addTaskUnlessCancelled(operation: sending @escaping @isolated(any) () async -> Void) -> Bool
```

## Parameters 

`operation`  

The operation to execute as part of the task group.

## Return Value

`true` if the child task was added to the group; otherwise `false`.

