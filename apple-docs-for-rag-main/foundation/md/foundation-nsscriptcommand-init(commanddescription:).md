

- Foundation
- NSScriptCommand
-  init(commandDescription:) 

Initializer

# init(commandDescription:)

Returns an a script command object initialized from the passed command description.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(commandDescription commandDef: NSScriptCommandDescription)
```

## Parameters 

`commandDef`  

A command description for the command to be created.

## Return Value

A newly initialized instance of `NSScriptCommand` or a subclass.

## Discussion

To make this command object usable, you must set its receiving objects and arguments (if any) after invoking this method.

## See Also

### Related Documentation

Cocoa Scripting Guide

var receiversSpecifier: NSScriptObjectSpecifier?

Sets the object specifier to `receiversSpec` that, when evaluated, indicates the receiver or receivers of the command.

var arguments: [String : Any]?

Sets the arguments of the command to `args`.

