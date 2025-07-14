

- Background Tasks
- BGTaskScheduler
-  register(forTaskWithIdentifier:using:launchHandler:) 

Instance Method

# register(forTaskWithIdentifier:using:launchHandler:)

Register a launch handler for the task with the associated identifier that’s executed on the specified queue.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
func register(
    forTaskWithIdentifier identifier: String,
    using queue: dispatch_queue_t?,
    launchHandler: @escaping (BGTask) -> Void
) -> Bool
```

## Parameters 

`identifier`  

A string containing the identifier of the task.

`queue`  

A queue for executing the task. Pass `nil` to use a default background queue.

`launchHandler`  

The system runs the block of code for the launch handler when it launches the app in the background. The block takes a single parameter, a BGTask object used for assigning an expiration handler and for setting a completion status. The block has no return value.

## Return value

Returns true if the launch handler was registered. Returns false if the identifier isn’t included in the BGTaskSchedulerPermittedIdentifiers `Info.plist`.

## Discussion

Every identifier in the BGTaskSchedulerPermittedIdentifiers requires a handler. Registration of all launch handlers must be complete before the end of applicationDidFinishLaunching(_:).

Important

Register each task identifier only once. The system kills the app on the second registration of the same task identifier.

## See Also

### Scheduling a task

func submit(BGTaskRequest) throws

Submit a previously registered background task for execution.

