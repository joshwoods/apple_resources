

- Core Data
- NSPersistentStoreCoordinator
-  performAndWait(\_:) 

Instance Method

# performAndWait(\_:)

Executes the provided closure on the coordinator’s queue and waits for it to finish.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func performAndWait(_ block: () throws -> T) rethrows -> T
```

## Parameters 

`block`  

The closure to execute.

## See Also

### Performing tasks

func perform&lt;T>(() throws -> T) async rethrows -> T

Executes the provided closure asynchronously on the coordinator’s queue and awaits the result.

func perform(() -> Void)

Executes the provided closure asynchronously on the coordinator’s queue.

Deprecated

func performAndWait(() -> Void)

Executes the provided closure on the coordinator’s queue and waits for it to finish.

Deprecated

func execute(NSPersistentStoreRequest, with: NSManagedObjectContext) throws -> Any

Executes the specified request on each of the coordinator’s persistent stores.

