

- Core Data
- NSPersistentStoreCoordinator
-  performAndWait(\_:) Deprecated

Instance Method

# performAndWait(\_:)

Executes the provided closure on the coordinator’s queue and waits for it to finish.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func performAndWait(_ block: () -> Void)
```

Deprecated

Use performAndWait(_:) instead.

## Parameters 

`block`  

The closure to execute.

## See Also

### Performing tasks

func perform&lt;T>(() throws -> T) async rethrows -> T

Executes the provided closure asynchronously on the coordinator’s queue and awaits the result.

func performAndWait&lt;T>(() throws -> T) rethrows -> T

Executes the provided closure on the coordinator’s queue and waits for it to finish.

func perform(() -> Void)

Executes the provided closure asynchronously on the coordinator’s queue.

Deprecated

func execute(NSPersistentStoreRequest, with: NSManagedObjectContext) throws -> Any

Executes the specified request on each of the coordinator’s persistent stores.

