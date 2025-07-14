

- Core Data
- NSFetchRequest
-  propertiesToFetch 

Instance Property

# propertiesToFetch

A collection of either property descriptions or string property names that specify which properties should be returned by the fetch.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var propertiesToFetch: [Any]? { get set }
```

## Discussion

Property descriptions can either be instances of NSPropertyDescription or NSString. The property descriptions may represent attributes, to-one relationships, or expressions. The name of an attribute or relationship description must match the name of a description on the fetch request’s entity.

### Special Considerations

You must set the entity for the fetch request before setting this value; otherwise, NSFetchRequest throws an invalidArgumentException exception.

This property can be set with managedObjectResultType and thereby implement a partial faulting (whereby only some of the properties are populated) of the returned objects, as well as the dictionaryResultType to define what properties are included in the resulting NSDictionary.

## See Also

### Managing How Results Are Returned

var resultType: NSFetchRequestResultType

The result type of the fetch request.

var includesPendingChanges: Bool

A Boolean value that indicates whether, when the fetch is executed, it matches against currently unsaved changes in the managed object context.

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

