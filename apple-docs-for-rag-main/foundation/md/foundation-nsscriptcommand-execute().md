

- Foundation
- NSScriptCommand
-  execute() 

Instance Method

# execute()

Executes the command if it is valid and returns the result, if any.

Mac Catalyst 13.0+macOS 10.0+

``` source
func execute() -> Any?
```

## Discussion

Before this method executes the command (through `NSInvocation` mechanisms), it evaluates all object specifiers involved in the command, validates that the receivers can actually handle the command, and verifies that the types of any arguments that were initially object specifiers are valid.

You shouldn’t have to override this method. If the command’s receivers want to handle the command themselves, this method invokes their defined handler. Otherwise, it invokes performDefaultImplementation().

## See Also

### Related Documentation

var evaluatedReceivers: Any?

Returns the object or objects to which the command is to be sent (called both the “receivers” or “targets” of script commands).

var evaluatedArguments: [String : Any]?

Returns a dictionary containing the arguments of the command, evaluated from object specifiers to objects if necessary. The keys in the dictionary are the argument names.

### Executing the command

func performDefaultImplementation() -> Any?

Overridden by subclasses to provide a default implementation for the command represented by the receiver.

