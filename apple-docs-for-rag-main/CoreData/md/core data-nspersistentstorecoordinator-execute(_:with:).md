

- Core Data
- NSPersistentStoreCoordinator
-  execute(\_:with:) 

Instance Method

# execute(\_:with:)

Executes the specified request on each of the coordinator’s persistent stores.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func execute(
    _ request: NSPersistentStoreRequest,
    with context: NSManagedObjectContext
) throws -> Any
```

## Parameters 

`request`  

A fetch or save request.

`context`  

The context against which `request` should be executed.

## Return Value

An array containing managed objects, managed object IDs, or dictionaries as appropriate for a fetch request; an empty array if `request` is a save request, or `nil` if an error occurred.

## Discussion

User defined requests return arrays of arrays, where a nested array is the result returned from a single store.

## See Also

### Performing tasks

func perform&lt;T>(() throws -> T) async rethrows -> T

Executes the provided closure asynchronously on the coordinator’s queue and awaits the result.

func performAndWait&lt;T>(() throws -> T) rethrows -> T

Executes the provided closure on the coordinator’s queue and waits for it to finish.

func perform(() -> Void)

Executes the provided closure asynchronously on the coordinator’s queue.

Deprecated

func performAndWait(() -> Void)

Executes the provided closure on the coordinator’s queue and waits for it to finish.

Deprecated

