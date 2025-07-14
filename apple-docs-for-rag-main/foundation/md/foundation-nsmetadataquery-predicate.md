

- Foundation
- NSMetadataQuery
-  predicate 

Instance Property

# predicate

The predicate used to filter query results.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var predicate: NSPredicate? { get set }
```

## Discussion

Setting this property while a query is running stops the query and discards the current results. The receiver immediately starts a new query.

## See Also

### Configuring Queries

var searchScopes: [Any]

An array containing the search scopes.

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

var searchItems: [Any]?

An array of objects that define the query’s scope.

