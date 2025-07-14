

- Core Data
- NSFetchRequest
-  includesPendingChanges 

Instance Property

# includesPendingChanges

A Boolean value that indicates whether, when the fetch is executed, it matches against currently unsaved changes in the managed object context.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var includesPendingChanges: Bool { get set }
```

## Discussion

This value is true if when the fetch is executed, the fetch will match against currently unsaved changes in the managed object context; otherwise the value is false. The default value is true.

If the value is false, the fetch request doesn’t check unsaved changes and only returns objects that matched the predicate in the persistent store.

### Special Considerations

A value of true is not supported in conjunction with the result type dictionaryResultType, including calculation of aggregate results (such as `max` and `min`). For dictionaries, the array returned from the fetch reflects the current state in the persistent store, and does not take into account any pending changes, insertions, or deletions in the context.

If you need to take pending changes into account for some simple aggregations like `max` and `min`, you can instead use a normal fetch request, sorted on the attribute you want, with a fetch limit of 1.

## See Also

### Managing How Results Are Returned

var resultType: NSFetchRequestResultType

The result type of the fetch request.

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

