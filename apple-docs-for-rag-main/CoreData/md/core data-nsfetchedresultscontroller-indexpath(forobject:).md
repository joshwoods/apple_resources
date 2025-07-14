

- Core Data
- NSFetchedResultsController
-  indexPath(forObject:) 

Instance Method

# indexPath(forObject:)

Returns the index path of a given object.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func indexPath(forObject object: ResultType) -> IndexPath?
```

## Parameters 

`object`  

An object in the receiver’s fetch results.

## Return Value

The index path of `object` in the receiver’s fetch results, or `nil` if `object` could not be found.

## Discussion

In versions of iOS before 3.2, this method raises an exception if `object` is not contained in the receiver’s fetch results.

## See Also

### Accessing Results

var fetchedObjects: [ResultType]?

The results of the fetch.

func object(at: IndexPath) -> ResultType

Returns the object at the given index path in the fetch results.

