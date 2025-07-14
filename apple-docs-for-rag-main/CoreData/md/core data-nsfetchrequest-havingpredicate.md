

- Core Data
- NSFetchRequest
-  havingPredicate 

Instance Property

# havingPredicate

The predicate used to filter rows being returned by a query containing a GROUP BY directive.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var havingPredicate: NSPredicate? { get set }
```

## Discussion

If a `havingPredicate` value is supplied, the predicate will be run after. Specifying a `havingPredicate` requires that propertiesToGroupBy also be specified.

## See Also

### Related Documentation

class NSFetchRequest

A description of search criteria used to retrieve data from a persistent store.

### Grouping and Filtering Dictionary Results

var propertiesToGroupBy: [Any]?

An array of objects that indicates how data should be grouped before a select statement is run in a SQL database.

