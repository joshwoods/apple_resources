

- Core Data
- NSManagedObjectContext
-  NSManagedObjectContext.ScheduledTaskType 

Enumeration

# NSManagedObjectContext.ScheduledTaskType

The different types of scheduled tasks.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
enum ScheduledTaskType
```

## Topics

### Scheduled Task Types

case enqueued

The enqueued scheduled task type.

case immediate

The immediate scheduled task type.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Performing block operations

func perform(() -> Void)

Asynchronously performs the specified closure on the context’s queue.

func perform&lt;T>(schedule: NSManagedObjectContext.ScheduledTaskType, () throws -> T) async rethrows -> T

Submits a closure to the context’s queue for asynchronous execution.

func performAndWait(() -> Void)

Synchronously performs the specified closure on the context’s queue.

func performAndWait&lt;T>(() throws -> T) rethrows -> T

Submits a closure to the context’s queue for synchronous execution.

