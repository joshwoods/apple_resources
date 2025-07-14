

- Foundation
- NSScriptClassDescription
-  supportsCommand(\_:) 

Instance Method

# supportsCommand(\_:)

Returns a Boolean value indicating whether the receiver or any superclass supports the specified command.

Mac Catalyst 13.0+macOS 10.0+

``` source
func supportsCommand(_ commandDescription: NSScriptCommandDescription) -> Bool
```

## Parameters 

`commandDescription`  

A description for a script command, such as `duplicate`, `make`, or `move`. Encapsulates the scriptability information for that command, such as its Objective-C selector, its argument names and types, and its return type (if any).

## Return Value

true if an the receiver or the instance of `NSScriptClassDescription` of any superclass of the receiver’s class lists the command described by `commandDesc` among its supported commands; otherwise, false.

## See Also

### Getting command information

func selector(forCommand: NSScriptCommandDescription) -> Selector?

Returns the selector associated with the receiver for the specified command description.

