

- Foundation
- NSScriptObjectSpecifier
-  containerClassDescription 

Instance Property

# containerClassDescription

Sets the class description of the receiver’s container specifier to a given specifier.

Mac Catalyst 13.0+macOS 10.0+

``` source
var containerClassDescription: NSScriptClassDescription? { get set }
```

## Parameters 

`classDescription`  

The class description of the receiver’s container specifier.

## See Also

### Getting, testing, and setting containers

var containerIsObjectBeingTested: Bool

Sets whether the receiver’s container should be an object involved in a filter reference or the top-level object.

var containerIsRangeContainerObject: Bool

Sets whether the receiver’s container is to be the container for a range specifier or a top-level object.

var container: NSScriptObjectSpecifier?

Sets the container specifier of the receiver.

