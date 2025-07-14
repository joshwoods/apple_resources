

- Foundation
- NSScriptCommand
-  evaluatedReceivers 

Instance Property

# evaluatedReceivers

Returns the object or objects to which the command is to be sent (called both the “receivers” or “targets” of script commands).

Mac Catalyst 13.0+macOS 10.0+

``` source
var evaluatedReceivers: Any? { get }
```

## Discussion

It evaluates receivers, which are always object specifiers, to a proper object. If the command does not specify a receiver, or if the receiver doesn’t accept the command, it returns `nil`.

## See Also

### Accessing receivers

var receiversSpecifier: NSScriptObjectSpecifier?

Sets the object specifier to `receiversSpec` that, when evaluated, indicates the receiver or receivers of the command.

