

- Core Data
- NSFetchRequest
-  resultType 

Instance Property

# resultType

The result type of the fetch request.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var resultType: NSFetchRequestResultType { get set }
```

## Discussion

The default value is managedObjectResultType.

If you set the value to managedObjectIDResultType, and do not include property values in the request, sort orderings are demoted to “best efforts” hints.

includesPendingChanges discusses with whether pending changes are taken into account when the `resultType` is set to `managedObjectResultType`.

includesPropertyValues discusses whether property values are included or not by default when the `resultType` is set to `managedObjectResultType`.

## See Also

### Managing How Results Are Returned

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

var returnsObjectsAsFaults: Bool

A Boolean value that indicates whether the objects resulting from a fetch request are faults.

struct NSFetchRequestResultType

Constants that specify the possible result types a fetch request can return.

protocol NSFetchRequestResult

An abstract protocol used with parameterized fetch requests.

