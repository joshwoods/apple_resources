

- Core Data
- NSFetchedResultsController
-  fetchedObjects 

Instance Property

# fetchedObjects

The results of the fetch.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var fetchedObjects: [ResultType]? { get }
```

## Discussion

The value of the property is `nil` if performFetch() hasn’t been called.

The results array only includes instances of the entity specified by the fetch request (fetchRequest) and that match its predicate. (If the fetch request has no predicate, then the results array includes all instances of the entity specified by the fetch request.)

The results array reflects the in-memory state of managed objects in the controller’s managed object context, not their state in the persistent store. The returned array does not, however, update as managed objects are inserted, modified, or deleted.

## See Also

### Related Documentation

func fetch(NSFetchRequest&lt;any NSFetchRequestResult>) throws -> [Any]

Returns an array of objects that meet the criteria of the specified fetch request.

### Accessing Results

func object(at: IndexPath) -> ResultType

Returns the object at the given index path in the fetch results.

func indexPath(forObject: ResultType) -> IndexPath?

Returns the index path of a given object.

