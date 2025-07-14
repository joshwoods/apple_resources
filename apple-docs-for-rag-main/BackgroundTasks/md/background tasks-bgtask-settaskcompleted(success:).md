

- Background Tasks
- BGTask
-  setTaskCompleted(success:) 

Instance Method

# setTaskCompleted(success:)

Informs the background task scheduler that the task is complete.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
func setTaskCompleted(success: Bool)
```

## Parameters 

`success`  

A `Boolean` indicating if the task completed successfully or not.

## Mentioned in 

Choosing Background Strategies for Your App

## Discussion

Not calling setTaskCompleted(success:) before the time for the task expires may result in the system killing your app.

You can reschedule an unsuccessful required task.

Important

If you don’t set an expiration handler, the system will mark your task as complete and unsuccessful instead of sending a warning.

## See Also

### Configuring a Task

var expirationHandler: (() -> Void)?

A handler called shortly before the task’s background time expires.

