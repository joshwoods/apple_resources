

- Foundation
- Process
-  didTerminateNotification 

Type Property

# didTerminateNotification

Posted when the task has stopped execution.

Mac Catalyst 13.0+macOS 10.0+

``` source
class let didTerminateNotification: NSNotification.Name
```

## Discussion

The notification object is the `NSTask` object that the system terminated. This notification doesn’t contain a `userInfo` dictionary.

The system posts this notification from the thread in which the `NSTask` object called launch(). When launching a task from a secondary thread or background queue, you can use the terminationHandler property instead for greater control over the execution context of any operations to be performed after the task finishes.

This notification can be posted either when the task has exited normally or as a result of terminate() being sent to the `NSTask` object. If the `NSTask` object gets released, however, this notification won’t get sent, as the port the message would have been sent on was released as part of the task release. The observer method can use terminationStatus to determine why the task died.

