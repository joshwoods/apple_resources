

- Foundation
- NSScriptObjectSpecifier
-  indicesOfObjectsByEvaluating(withContainer:count:) 

Instance Method

# indicesOfObjectsByEvaluating(withContainer:count:)

This primitive method must be overridden by subclasses to return a pointer to an array of indices identifying objects in the key of a given container that are identified by the receiver of the message.

Mac Catalyst 13.0+macOS 10.0+

``` source
func indicesOfObjectsByEvaluating(
    withContainer container: Any,
    count: UnsafeMutablePointer
) -> UnsafeMutablePointer?
```

## Discussion

This primitive method must be overridden by subclasses to return a pointer to an array of indices identifying objects in the key of the container `aContainer` that are identified by the receiver of the message. The method uses key-value coding to obtain values based on the receiver’s key. It returns the number of such matching objects by indirection in `numRefs`. It returns `nil` directly and –1 via `numRefs` if all objects in the container (or the sole object) match the value of the receiver’s key. This method is invoked by objectsByEvaluating(withContainers:). The default implementation returns `nil` directly and –1 indirectly via `numRefs`.

## See Also

### Evaluating an object specifier

var objectsByEvaluatingSpecifier: Any?

Returns the actual object represented by the nested series of object specifiers.

func objectsByEvaluating(withContainers: Any) -> Any?

Returns the actual object or objects specified by the receiver as evaluated in the context of given container object.

