

- Foundation
- NSMetadataQuery
-  delegate 

Instance Property

# delegate

The query’s delegate.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
unowned(unsafe) var delegate: (any NSMetadataQueryDelegate)? { get set }
```

## Discussion

This property contains an object that acts as the query’s delegate, or `nil`. The delegate must implement the NSMetadataQueryDelegate. Pass `nil` to remove the current delegate.

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

var searchItems: [Any]?

An array of objects that define the query’s scope.

