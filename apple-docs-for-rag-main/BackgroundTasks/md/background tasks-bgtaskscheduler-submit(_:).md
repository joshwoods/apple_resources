

- Background Tasks
- BGTaskScheduler
-  submit(\_:) 

Instance Method

# submit(\_:)

Submit a previously registered background task for execution.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
func submit(_ taskRequest: BGTaskRequest) throws
```

## Parameters 

`taskRequest`  

A background task request object specifying the task identifier and optional configuration information.

## Mentioned in 

Starting and Terminating Tasks During Development

## Discussion

Submitting a task request for an unexecuted task that’s already in the queue replaces the previous task request.

There can be a total of 1 refresh task and 10 processing tasks scheduled at any time. Trying to schedule more tasks returns BGTaskScheduler.Error.Code.tooManyPendingTaskRequests.

## See Also

### Scheduling a task

func register(forTaskWithIdentifier: String, using: dispatch_queue_t?, launchHandler: (BGTask) -> Void) -> Bool

Register a launch handler for the task with the associated identifier that’s executed on the specified queue.

