

- Foundation
- NSScriptCommand
-  receiversSpecifier 

Instance Property

# receiversSpecifier

Sets the object specifier to `receiversSpec` that, when evaluated, indicates the receiver or receivers of the command.

Mac Catalyst 13.0+macOS 10.0+

``` source
var receiversSpecifier: NSScriptObjectSpecifier? { get set }
```

## Discussion

If you create a subclass of `NSScriptCommand`, you don’t necessarily need to override this method, though some of Cocoa’s subclasses do. An override should perform the same function as the superclass method, with a critical difference: it causes the container specifier part of the passed-in object specifier to become the receiver specifier of the command, and the key part of the passed-in object specifier to become the key specifier. In an override, for example, if `receiversRef` is a specifier for `the third rectangle of the first document`, the receiver specifier is `the first document` while the key specifier is `the third rectangle`.

## See Also

### Accessing receivers

var evaluatedReceivers: Any?

Returns the object or objects to which the command is to be sent (called both the “receivers” or “targets” of script commands).

