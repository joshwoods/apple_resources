

- Foundation
- NSCloneCommand
-  keySpecifier 

Instance Property

# keySpecifier

Returns a specifier for the object or objects to be cloned.

Mac Catalyst 13.0+macOS 10.0+

``` source
var keySpecifier: NSScriptObjectSpecifier { get }
```

## Return Value

A specifier for the object or objects to be cloned.

## Discussion

For example, the specifier may indicate that a document’s third rectangle should be cloned. The returned specifier is valid only in the context of the `NSCloneCommand` object; for example, if you send the specifier a container message, the result is `nil`.

## See Also

### Related Documentation

Cocoa Scripting Guide

### Working with specifiers

func setReceiversSpecifier(NSScriptObjectSpecifier?)

Sets the receiver’s object specifier;.

