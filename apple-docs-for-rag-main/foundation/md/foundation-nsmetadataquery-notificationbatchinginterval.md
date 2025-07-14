

- Foundation
- NSMetadataQuery
-  notificationBatchingInterval 

Instance Property

# notificationBatchingInterval

The interval at which notification of updated results occurs.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var notificationBatchingInterval: TimeInterval { get set }
```

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

var delegate: (any NSMetadataQueryDelegate)?

The query’s delegate.

var searchItems: [Any]?

An array of objects that define the query’s scope.

