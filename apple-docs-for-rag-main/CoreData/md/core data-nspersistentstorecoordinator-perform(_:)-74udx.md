

- Core Data
- NSPersistentStoreCoordinator
-  perform(\_:) 

Instance Method

# perform(\_:)

Executes the provided closure asynchronously on the coordinator’s queue and awaits the result.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func perform(_ block: @escaping () throws -> T) async rethrows -> T
```

## Parameters 

`block`  

The closure to execute.

## See Also

### Performing tasks

func performAndWait&lt;T>(() throws -> T) rethrows -> T

Executes the provided closure on the coordinator’s queue and waits for it to finish.

func perform(() -> Void)

Executes the provided closure asynchronously on the coordinator’s queue.

Deprecated

func performAndWait(() -> Void)

Executes the provided closure on the coordinator’s queue and waits for it to finish.

Deprecated

func execute(NSPersistentStoreRequest, with: NSManagedObjectContext) throws -> Any

Executes the specified request on each of the coordinator’s persistent stores.

