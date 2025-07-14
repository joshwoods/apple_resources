

- Core Data
- NSFetchedResultsController
-  init(fetchRequest:managedObjectContext:sectionNameKeyPath:cacheName:) 

Initializer

# init(fetchRequest:managedObjectContext:sectionNameKeyPath:cacheName:)

Returns a fetch request controller initialized using the given arguments.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(
    fetchRequest: NSFetchRequest,
    managedObjectContext context: NSManagedObjectContext,
    sectionNameKeyPath: String?,
    cacheName name: String?
)
```

## Parameters 

`fetchRequest`  

The fetch request used to get the objects.

The fetch request must have at least one sort descriptor. If the controller generates sections, the first sort descriptor in the array is used to group the objects into sections; its key must either be the same as `sectionNameKeyPath` or the relative ordering using its key must match that using `sectionNameKeyPath`.

Important

You must not modify `fetchRequest` after invoking this method. For example, you must not change its predicate or the sort orderings.

`context`  

The managed object against which `fetchRequest` is executed.

`sectionNameKeyPath`  

A key path on result objects that returns the section name. Pass `nil` to indicate that the controller should generate a single section.

The section name is used to pre-compute the section information.

If this key path is not the same as that specified by the first sort descriptor in `fetchRequest`, they must generate the same relative orderings. For example, the first sort descriptor in `fetchRequest` might specify the key for a persistent property; `sectionNameKeyPath` might specify a key for a transient property derived from the persistent property.

`name`  

The name of the cache file the receiver should use. Pass `nil` to prevent caching.

Pre-computed section info is cached to a private directory under this name. If Core Data finds a cache stored with this name, it is checked to see if it matches the `fetchRequest`. If it does, the cache is loaded directly—this avoids the overhead of computing the section and index information. If the cached information doesn’t match the request, the cache is deleted and recomputed when the fetch happens.

## Return Value

The receiver initialized with the specified fetch request, context, key path, and cache name.

## See Also

### Related Documentation

Core Data Programming Guide

### Initializing a Fetched Results Controller

func performFetch() throws

Executes the controller’s fetch request.

