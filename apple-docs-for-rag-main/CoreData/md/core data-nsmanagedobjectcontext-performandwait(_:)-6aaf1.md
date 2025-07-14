

- Core Data
- NSManagedObjectContext
-  performAndWait(\_:) 

Instance Method

# performAndWait(\_:)

Submits a closure to the context’s queue for synchronous execution.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func performAndWait(_ block: () throws -> T) rethrows -> T
```

## Parameters 

`block`  

The closure to perform.

## Discussion

This method supports *reentrancy* — meaning it’s safe to call the method again, from within the closure, before the previous invocation completes.

## See Also

### Performing block operations

func perform(() -> Void)

Asynchronously performs the specified closure on the context’s queue.

func perform&lt;T>(schedule: NSManagedObjectContext.ScheduledTaskType, () throws -> T) async rethrows -> T

Submits a closure to the context’s queue for asynchronous execution.

func performAndWait(() -> Void)

Synchronously performs the specified closure on the context’s queue.

enum ScheduledTaskType

The different types of scheduled tasks.

