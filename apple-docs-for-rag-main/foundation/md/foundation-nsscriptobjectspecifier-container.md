

- Foundation
- NSScriptObjectSpecifier
-  container 

Instance Property

# container

Sets the container specifier of the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var container: NSScriptObjectSpecifier? { get set }
```

## Parameters 

`objSpecifier`  

The container specifier for the receiver.

## See Also

### Getting, testing, and setting containers

var containerClassDescription: NSScriptClassDescription?

Sets the class description of the receiver’s container specifier to a given specifier.

var containerIsObjectBeingTested: Bool

Sets whether the receiver’s container should be an object involved in a filter reference or the top-level object.

var containerIsRangeContainerObject: Bool

Sets whether the receiver’s container is to be the container for a range specifier or a top-level object.

