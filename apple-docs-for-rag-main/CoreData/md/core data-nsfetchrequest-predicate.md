

- Core Data
- NSFetchRequest
-  predicate 

Instance Property

# predicate

The predicate of the fetch request.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var predicate: NSPredicate? { get set }
```

## Discussion

The predicate instance constrains the selection of objects the NSFetchRequest instance is to fetch.

If the predicate is empty—for example, if it is an `AND` predicate whose array of elements contains no predicates—the request has its predicate set to `nil`. For more about predicates, see Predicate Programming Guide.

## See Also

### Specifying Fetch Constraints

var fetchLimit: Int

The fetch limit of the fetch request.

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

