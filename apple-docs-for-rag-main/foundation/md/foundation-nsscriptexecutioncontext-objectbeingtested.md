

- Foundation
- NSScriptExecutionContext
-  objectBeingTested 

Instance Property

# objectBeingTested

Sets the top-level container object currently being tested in a “whose” qualifier to a given object.

Mac Catalyst 13.0+macOS 10.0+

``` source
var objectBeingTested: Any? { get set }
```

## Parameters 

`object`  

The top-level container object currently being tested.

## See Also

### Getting and setting the container object

var topLevelObject: Any?

Sets the top-level object for an object-specifier evaluation.

var rangeContainerObject: Any?

Sets the top-level container object for a range-specifier evaluation to a give object.

