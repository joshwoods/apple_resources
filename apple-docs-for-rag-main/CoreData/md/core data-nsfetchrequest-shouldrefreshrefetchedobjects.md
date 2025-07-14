

- Core Data
- NSFetchRequest
-  shouldRefreshRefetchedObjects 

Instance Property

# shouldRefreshRefetchedObjects

A Boolean value that indicates whether the property values of fetched objects will be updated with the current values in the persistent store.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var shouldRefreshRefetchedObjects: Bool { get set }
```

## Discussion

This value is true if the property values of fetched objects will be updated with the current values in the persistent store; otherwise, it is false.

By default when you fetch objects, they maintain their current property values, even if the values in the persistent store have changed. Invoking this method with the parameter true means that when the fetch is executed, the property values of fetched objects are updated with the current values in the persistent store. This is a more convenient way to ensure that managed object property values are consistent with the store than by using refresh(_:mergeChanges:) (`NSManagedObjetContext`) for multiple objects in turn.

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

var returnsObjectsAsFaults: Bool

A Boolean value that indicates whether the objects resulting from a fetch request are faults.

struct NSFetchRequestResultType

Constants that specify the possible result types a fetch request can return.

protocol NSFetchRequestResult

An abstract protocol used with parameterized fetch requests.

