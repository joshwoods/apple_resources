

- Core Data
- NSFetchRequest
-  includesPropertyValues 

Instance Property

# includesPropertyValues

A Boolean value that indicates whether, when the fetch is executed, property data is obtained from the persistent store.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var includesPropertyValues: Bool { get set }
```

## Discussion

This value is true if when the fetch is executed, property data is obtained from the persistent store; otherwise it is false. The default value is true.

You can set includesPropertyValues to false to avoid creating objects to represent property values and thereby reduce memory overhead. You typically should only do so, however, if you are sure that you will not need the actual property data, or you already have the information in the row cache. Otherwise, you will incur multiple trips to the database.

During a normal fetch (includesPropertyValues is true), Core Data fetches the object ID *and* property data for the matching records, fills the row cache with the information, and returns managed objects as faults (see returnsObjectsAsFaults). Although these faults are managed objects, all of their property data still resides in the row cache until the fault is fired. When the fault is fired, Core Data retrieves the data from the row cache—there is no need to go back to the database.

If includesPropertyValues is false, then Core Data fetches *only* the object ID information for the matching records—it does not populate the row cache. Core Data still returns managed objects because it only needs managed object IDs to create faults. However, if you subsequently fire the fault, Core Data looks in the (empty) row cache, doesn’t find any data, and then goes back to the store a second time for the data.

If includesPropertyValues is true and resultType is set to managedObjectIDResultType, the properties are fetched even though they are not being presented to the application and can result in a significant performance penalty.

## See Also

### Managing How Results Are Returned

var resultType: NSFetchRequestResultType

The result type of the fetch request.

var includesPendingChanges: Bool

A Boolean value that indicates whether, when the fetch is executed, it matches against currently unsaved changes in the managed object context.

var propertiesToFetch: [Any]?

A collection of either property descriptions or string property names that specify which properties should be returned by the fetch.

var returnsDistinctResults: Bool

A Boolean value that indicates whether the fetch request returns only distinct values for the fields specified by propertiesToFetch.

var shouldRefreshRefetchedObjects: Bool

A Boolean value that indicates whether the property values of fetched objects will be updated with the current values in the persistent store.

var returnsObjectsAsFaults: Bool

A Boolean value that indicates whether the objects resulting from a fetch request are faults.

struct NSFetchRequestResultType

Constants that specify the possible result types a fetch request can return.

protocol NSFetchRequestResult

An abstract protocol used with parameterized fetch requests.

