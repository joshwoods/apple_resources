

- Core Data
- NSBatchUpdateRequest
-  predicate 

Instance Property

# predicate

A predicate that identifies the objects to update.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var predicate: NSPredicate? { get set }
```

## See Also

### Configuring a Request

var entity: NSEntityDescription

The managed entity to update data for.

var entityName: String

The name of the managed entity to update data for.

var includesSubentities: Bool

A Boolean value that indicates whether to update subentities.

var propertiesToUpdate: [AnyHashable : Any]?

A dictionary of property description pairs that describe the updates.

var resultType: NSBatchUpdateRequestResultType

The type of result that Core Data returns from the request.

