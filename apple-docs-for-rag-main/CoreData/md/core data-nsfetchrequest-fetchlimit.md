

- Core Data
- NSFetchRequest
-  fetchLimit 

Instance Property

# fetchLimit

The fetch limit of the fetch request.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var fetchLimit: Int { get set }
```

## Discussion

The fetch limit specifies the maximum number of objects that a request should return when executed.

If you set a fetch limit, the framework makes a best effort to improve efficiency, but does not guarantee it. For every object store except the SQL store, a fetch request executed with a fetch limit in effect simply performs an unlimited fetch and throws away the unasked for rows.

## See Also

### Specifying Fetch Constraints

var predicate: NSPredicate?

The predicate of the fetch request.

var fetchOffset: Int

The fetch offset of the fetch request.

var fetchBatchSize: Int

The batch size of the objects specified in the fetch request.

var affectedStores: [NSPersistentStore]?

An array of persistent stores specified for the fetch request.

class NSFetchRequestExpression

An expression that evaluates the result of a fetch request on a managed object context.

class NSExpressionDescription

An object that describes an expression to include with a fetch request.

class NSFetchedPropertyDescription

A description object used to define which properties are fetched from Core Data.

