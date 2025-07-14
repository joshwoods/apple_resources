

- Core Data
- NSManagedObjectContext
-  perform(schedule:\_:) 

Instance Method

# perform(schedule:\_:)

Submits a closure to the context’s queue for asynchronous execution.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func perform(
    schedule: NSManagedObjectContext.ScheduledTaskType = .immediate,
    _ block: @escaping () throws -> T
) async rethrows -> T
```

## Parameters 

`schedule`  

The required execution schedule. For more information, see NSManagedObjectContext.ScheduledTaskType.

`block`  

The closure to perform.

## See Also

### Performing block operations

func perform(() -> Void)

Asynchronously performs the specified closure on the context’s queue.

func performAndWait(() -> Void)

Synchronously performs the specified closure on the context’s queue.

func performAndWait&lt;T>(() throws -> T) rethrows -> T

Submits a closure to the context’s queue for synchronous execution.

enum ScheduledTaskType

The different types of scheduled tasks.

