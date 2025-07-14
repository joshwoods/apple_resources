

- Core Data
- NSManagedObjectContext
-  perform(\_:) 

Instance Method

# perform(\_:)

Asynchronously performs the specified closure on the context’s queue.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func perform(_ block: @escaping () -> Void)
```

## Parameters 

`block`  

The closure to perform.

## Mentioned in 

Using Core Data in the background

## Discussion

This method encapsulates an autorelease pool and a call to processPendingChanges().

## See Also

### Performing block operations

func perform&lt;T>(schedule: NSManagedObjectContext.ScheduledTaskType, () throws -> T) async rethrows -> T

Submits a closure to the context’s queue for asynchronous execution.

func performAndWait(() -> Void)

Synchronously performs the specified closure on the context’s queue.

func performAndWait&lt;T>(() throws -> T) rethrows -> T

Submits a closure to the context’s queue for synchronous execution.

enum ScheduledTaskType

The different types of scheduled tasks.

