

- Foundation
- NSScriptExecutionContext
-  rangeContainerObject 

Instance Property

# rangeContainerObject

Sets the top-level container object for a range-specifier evaluation to a give object.

Mac Catalyst 13.0+macOS 10.0+

``` source
var rangeContainerObject: Any? { get set }
```

## Parameters 

`container`  

The top-level container object for a range-specifier evaluation.

## Discussion

Instances of `NSRangeSpecifier` contain object specifiers representing the first or last element in a range of elements, and these specifiers are evaluated in the context of `container`.

## See Also

### Getting and setting the container object

var topLevelObject: Any?

Sets the top-level object for an object-specifier evaluation.

var objectBeingTested: Any?

Sets the top-level container object currently being tested in a “whose” qualifier to a given object.

