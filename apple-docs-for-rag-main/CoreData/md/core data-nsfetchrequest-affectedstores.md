

- Core Data
- NSFetchRequest
-  affectedStores 

Instance Property

# affectedStores

An array of persistent stores specified for the fetch request.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var affectedStores: [NSPersistentStore]? { get set }
```

## Discussion

The contents of the array are the identifiers for the stores to be searched when the fetch request is executed.

## See Also

### Specifying Fetch Constraints

var predicate: NSPredicate?

The predicate of the fetch request.

var fetchLimit: Int

The fetch limit of the fetch request.

var fetchOffset: Int

The fetch offset of the fetch request.

var fetchBatchSize: Int

The batch size of the objects specified in the fetch request.

class NSFetchRequestExpression

An expression that evaluates the result of a fetch request on a managed object context.

class NSExpressionDescription

An object that describes an expression to include with a fetch request.

class NSFetchedPropertyDescription

A description object used to define which properties are fetched from Core Data.

