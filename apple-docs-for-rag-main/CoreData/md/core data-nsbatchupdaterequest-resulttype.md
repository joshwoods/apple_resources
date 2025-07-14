

- Core Data
- NSBatchUpdateRequest
-  resultType 

Instance Property

# resultType

The type of result that Core Data returns from the request.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var resultType: NSBatchUpdateRequestResultType { get set }
```

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

var propertiesToUpdate: [AnyHashable : Any]?

A dictionary of property description pairs that describe the updates.

