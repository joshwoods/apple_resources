

- Core Data
-  NSFetchRequestResult 

Protocol

# NSFetchRequestResult

An abstract protocol used with parameterized fetch requests.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol NSFetchRequestResult : NSObjectProtocol
```

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSManagedObject
- NSManagedObjectID

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

var returnsObjectsAsFaults: Bool

A Boolean value that indicates whether the objects resulting from a fetch request are faults.

struct NSFetchRequestResultType

Constants that specify the possible result types a fetch request can return.

