

- Foundation
- NSMetadataQuery
-  searchScopes 

Instance Property

# searchScopes

An array containing the search scopes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var searchScopes: [Any] { get set }
```

## Discussion

This array can contain `NSURL` or `NSString` objects that represent file-system directories or the search scopes for the query. For a list of valid search scopes, see Metadata Query Search Scopes. An empty array indicates that there is no limitation on where the query searches.

## See Also

### Related Documentation

File Metadata Search Programming Guide

### Configuring Queries

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

var searchItems: [Any]?

An array of objects that define the query’s scope.

