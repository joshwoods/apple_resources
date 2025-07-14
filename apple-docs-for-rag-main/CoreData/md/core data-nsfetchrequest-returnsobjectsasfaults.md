

- Core Data
- NSFetchRequest
-  returnsObjectsAsFaults 

Instance Property

# returnsObjectsAsFaults

A Boolean value that indicates whether the objects resulting from a fetch request are faults.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var returnsObjectsAsFaults: Bool { get set }
```

## Discussion

This value is true if the objects resulting from a fetch using the NSFetchRequest are faults; otherwise, it is false. The default value is true. This setting is not used if the result type (see resultType) is `NSManagedObjectIDResultType`, as object IDs do not have property values. You can set returnsObjectsAsFaults to false to gain a performance benefit if you know you will need to access the property values from the returned objects.

When you execute a fetch, by default returnsObjectsAsFaults is true; Core Data fetches the object data for the matching records, fills the row cache with the information, and returns managed object as faults. These faults are managed objects, but all of their property data resides in the row cache until the fault is fired. When the fault is fired, Core Data retrieves the data from the row cache. Although the overhead for this operation is small, for large datasets it may not be trivial. If you *need* to access the property values from the returned objects (for example, if you iterate over all the objects to calculate the average value of a particular attribute), then it is more efficient to set returnsObjectsAsFaults to false to avoid the additional overhead.

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

var includesPropertyValues: Bool

A Boolean value that indicates whether, when the fetch is executed, property data is obtained from the persistent store.

var shouldRefreshRefetchedObjects: Bool

A Boolean value that indicates whether the property values of fetched objects will be updated with the current values in the persistent store.

struct NSFetchRequestResultType

Constants that specify the possible result types a fetch request can return.

protocol NSFetchRequestResult

An abstract protocol used with parameterized fetch requests.

