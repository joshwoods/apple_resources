

- WatchKit
- WKExtensionDelegate
-  handle(\_:) 

Instance Method

# handle(\_:)

Tells the delegate that the app has received one or more background tasks.

watchOS 3.0+

``` source
@MainActor
optional func handle(_ backgroundTasks: Set)
```

## Parameters 

`backgroundTasks`  

A set containing one or more background tasks.

## Mentioned in 

Using background tasks

## Discussion

The system calls this method after launching your app to handle a background task. Use this method to handle the specified tasks. Call each tasks’s setTaskCompletedWithSnapshot(_:) method as soon as the task is complete. For more information on background tasks, see Using background tasks.

## See Also

### Related Documentation

func recoverActiveWorkoutSession(completion: (HKWorkoutSession?, (any Error)?) -> Void)

Recovers an active workout session.

