

- Core Data
- NSFetchRequest
-  propertiesToGroupBy 

Instance Property

# propertiesToGroupBy

An array of objects that indicates how data should be grouped before a select statement is run in a SQL database.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var propertiesToGroupBy: [Any]? { get set }
```

## Discussion

An array of NSPropertyDescription or NSExpressionDescription objects or key-path strings that indicate how data should be grouped before a select statement is run in an SQL database.

If you use this setting, you must set the resultType to dictionaryResultType, and the SELECT values must be literals, aggregates, or columns specified in `propertiesToGroupBy`.

Aggregates will operate on the groups specified in `propertiesToGroupBy`

rather than the whole table. If you set `propertiesToGroupBy`, you can also set a predicate to filter rows that are returned by `propertiesToGroupBy`.

See havingPredicate.

## See Also

### Grouping and Filtering Dictionary Results

var havingPredicate: NSPredicate?

The predicate used to filter rows being returned by a query containing a GROUP BY directive.

