

- Core Data
- NSBatchUpdateRequest
-  propertiesToUpdate 

Instance Property

# propertiesToUpdate

A dictionary of property description pairs that describe the updates.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var propertiesToUpdate: [AnyHashable : Any]? { get set }
```

## Discussion

The dictionary keys are either NSPropertyDescription objects or strings that identify the property name.

The dictionary values are either a constant value or an NSExpression that evaluates to a scalar value.

## See Also

### Configuring a Request

var entity: NSEntityDescription

The managed entity to update data for.

var entityName: String

The name of the managed entity to update data for.

var includesSubentities: Bool

A Boolean value that indicates whether to update subentities.

var predicate: NSPredicate?

A predicate that identifies the objects to update.

var resultType: NSBatchUpdateRequestResultType

The type of result that Core Data returns from the request.

