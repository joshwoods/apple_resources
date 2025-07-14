

- Core Data
- NSManagedObjectContext
- NSManagedObjectContext.ScheduledTaskType
-  NSManagedObjectContext.ScheduledTaskType.enqueued 

Case

# NSManagedObjectContext.ScheduledTaskType.enqueued

The enqueued scheduled task type.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
case enqueued
```

## Discussion

Enqueued tasks execute asynchronously on the context’s queue. An enqueued task encapsulates an autorelease pool and a call to processPendingChanges(), and its behavior is analogous to perform(_:). The context’s queue executes tasks in the order you add them.

## See Also

### Scheduled Task Types

case immediate

The immediate scheduled task type.

