

- Foundation
- NSMetadataQuery
-  searchItems 

Instance Property

# searchItems

An array of objects that define the query’s scope.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var searchItems: [Any]? { get set }
```

## Discussion

Use this method to scope the metadata query to a collection of existing URLs and/or metadata items. This array contains the `NSURL` and/or `NSMetadataItem` items to be searched.

## See Also

### Configuring Queries

var searchScopes: [Any]

An array containing the search scopes.

var predicate: NSPredicate?

The predicate used to filter query results.

var sortDescriptors: [NSSortDescriptor]

An array of sort descriptor objects.

var valueListAttributes: [String]

An array of attributes whose values are gathered by the query.

var groupingAttributes: [String]?

An array of grouping attributes. (read-only)

var notificationBatchingInterval: TimeInterval

The interval at which notification of updated results occurs.

var delegate: (any NSMetadataQueryDelegate)?

The query’s delegate.

