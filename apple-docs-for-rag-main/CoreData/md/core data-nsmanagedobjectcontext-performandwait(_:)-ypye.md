

- Core Data
- NSManagedObjectContext
-  performAndWait(\_:) 

Instance Method

# performAndWait(\_:)

Synchronously performs the specified closure on the context’s queue.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func performAndWait(_ block: () -> Void)
```

## Parameters 

`block`  

The closure to perform.

## Mentioned in 

Using Core Data in the background

## Discussion

This method supports *reentrancy* — meaning it’s safe to call the method again, from within the closure, before the previous invocation completes.

## See Also

### Performing block operations

func perform(() -> Void)

Asynchronously performs the specified closure on the context’s queue.

func perform&lt;T>(schedule: NSManagedObjectContext.ScheduledTaskType, () throws -> T) async rethrows -> T

Submits a closure to the context’s queue for asynchronous execution.

func performAndWait&lt;T>(() throws -> T) rethrows -> T

Submits a closure to the context’s queue for synchronous execution.

enum ScheduledTaskType

The different types of scheduled tasks.

