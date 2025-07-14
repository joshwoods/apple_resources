

- Core Data
- NSManagedObjectContext
- NSManagedObjectContext.ScheduledTaskType
-  NSManagedObjectContext.ScheduledTaskType.immediate 

Case

# NSManagedObjectContext.ScheduledTaskType.immediate

The immediate scheduled task type.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
case immediate
```

## Discussion

Immediate tasks execute right away if the context operates within the current scope; otherwise, the context enqueues the task. Tasks of this type are reentrant, nonblocking, and continuation-aware.

## See Also

### Scheduled Task Types

case enqueued

The enqueued scheduled task type.

