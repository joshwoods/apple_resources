

- SwiftUI
- WidgetConfiguration
-  backgroundTask(\_:action:) 

Instance Method

# backgroundTask(\_:action:)

Runs the given action when the system provides a background task.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func backgroundTask(
    _ task: BackgroundTask,
    action: @escaping (D) async -> R
) -> some WidgetConfiguration where D : Sendable, R : Sendable
```

## Parameters 

`task`  

The type of task the action responds to.

`action`  

The closure that is called when the system provides a task matching the provided task.

## Discussion

When the system wakes your app or extension for one or more background tasks, it will call any actions associated with matching tasks. When your async actions return, the system will put your app back into a suspended state. In Widget Extensions, this modifier can be used to handle URL Session background tasks with urlSession.

## See Also

### Managing background tasks

func onBackgroundURLSessionEvents(matching:_:)

Adds an action to perform when events related to a URL session identified by a closure are waiting to be processed.

