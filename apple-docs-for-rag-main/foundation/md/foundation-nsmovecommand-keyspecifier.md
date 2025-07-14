

- Foundation
- NSMoveCommand
-  keySpecifier 

Instance Property

# keySpecifier

Returns a specifier for the object or objects to be moved.

Mac Catalyst 13.0+macOS 10.0+

``` source
var keySpecifier: NSScriptObjectSpecifier { get }
```

## Return Value

A specifier for the object or objects to be moved.

## Discussion

Note that this specifier may be different than the specifier set by setReceiversSpecifier(_:), which sets the container specifier. For example, for a command such as `move the third circle to the location of the first circle`, the receiver might identify a document (which has a list of graphics), while the key specifier identifies the particular graphic to be moved.

## See Also

### Related Documentation

Cocoa Scripting Guide

### Working with specifiers

func setReceiversSpecifier(NSScriptObjectSpecifier?)

Sets the receiver’s object specifier.

