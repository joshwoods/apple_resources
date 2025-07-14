

- Foundation
- NSScriptObjectSpecifier
-  containerIsRangeContainerObject 

Instance Property

# containerIsRangeContainerObject

Sets whether the receiver’s container is to be the container for a range specifier or a top-level object.

Mac Catalyst 13.0+macOS 10.0+

``` source
var containerIsRangeContainerObject: Bool { get set }
```

## Discussion

If the receiver’s container specifier is `nil` and `flag` is true, sets the receiver’s container to be the container for a range specifier. If the receiver’s container specifier is `nil` and `flag` is false, sets the receiver’s container to be the top-level object.

If `flag` is true, containerIsObjectBeingTested should not also be invoked with an argument of true.

## See Also

### Getting, testing, and setting containers

var containerClassDescription: NSScriptClassDescription?

Sets the class description of the receiver’s container specifier to a given specifier.

var containerIsObjectBeingTested: Bool

Sets whether the receiver’s container should be an object involved in a filter reference or the top-level object.

var container: NSScriptObjectSpecifier?

Sets the container specifier of the receiver.

