

- Foundation
- NSDeleteCommand
-  keySpecifier 

Instance Property

# keySpecifier

Returns a specifier for the object or objects to be deleted.

Mac Catalyst 13.0+macOS 10.0+

``` source
var keySpecifier: NSScriptObjectSpecifier { get }
```

## Return Value

A specifier for the object or objects to be deleted.

## Discussion

Note that this may be different than the specifier or specifiers set by setReceiversSpecifier(_:).

## See Also

### Related Documentation

Cocoa Scripting Guide

Key-Value Coding Programming Guide

### Working with specifiers

func setReceiversSpecifier(NSScriptObjectSpecifier?)

Sets the receiver’s object specifier.

