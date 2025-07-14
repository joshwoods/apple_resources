

- Core Data
- NSFetchedResultsController
-  object(at:) 

Instance Method

# object(at:)

Returns the object at the given index path in the fetch results.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func object(at indexPath: IndexPath) -> ResultType
```

## Parameters 

`indexPath`  

An index path in the fetch results.

If `indexPath` does not describe a valid index path in the fetch results, an exception is raised.

## Return Value

The object at a given index path in the fetch results.

## See Also

### Accessing Results

var fetchedObjects: [ResultType]?

The results of the fetch.

func indexPath(forObject: ResultType) -> IndexPath?

Returns the index path of a given object.

