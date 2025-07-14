

- Foundation
- NSMoveCommand
-  setReceiversSpecifier(\_:) 

Instance Method

# setReceiversSpecifier(\_:)

Sets the receiver’s object specifier.

Mac Catalyst 13.0+macOS 10.0+

``` source
func setReceiversSpecifier(_ receiversRef: NSScriptObjectSpecifier?)
```

## Parameters 

`receiversRef`  

The receiver’s object specifier.

## Discussion

When evaluated, `receiversRef` indicates the receiver or receivers of the `move` AppleScript command.

This method overrides receiversSpecifier in NSScriptCommand. It performs the same function as the overridden method, with a critical difference: it causes the container specifier part of the passed-in object specifier to become the receiver specifier of the command, and the key part of the passed-in object specifier to become the key specifier. If, for example, `receiversRef` is a specifier for `the third paragraph of the first document`, the receiver specifier is `the first document` while the key specifier is `the third paragraph`.

## See Also

### Working with specifiers

var keySpecifier: NSScriptObjectSpecifier

Returns a specifier for the object or objects to be moved.

