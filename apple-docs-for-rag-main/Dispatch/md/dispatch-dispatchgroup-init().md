

- Dispatch
- DispatchGroup
-  init() 

Initializer

# init()

Creates a new group to which you can assign block objects.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init()
```

## Return Value

The newly created group. In Objective-C returns `NULL` on failure.

## Discussion

This function creates a new group with which block objects can be associated (by using the dispatch_group_async function). The dispatch group maintains a count of its outstanding associated tasks, incrementing the count when a new task is associated and decrementing it when a task completes. Functions such as dispatch_group_notify and dispatch_group_wait use that count to allow your application to determine when all tasks associated with the group have completed. At that time, your application can take any appropriate action.

