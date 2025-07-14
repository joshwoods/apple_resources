

- Foundation
- NSScriptCommand
-  performDefaultImplementation() 

Instance Method

# performDefaultImplementation()

Overridden by subclasses to provide a default implementation for the command represented by the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func performDefaultImplementation() -> Any?
```

## Discussion

Do not invoke this method directly. execute() invokes this method when the command being executed is not supported by the class of the objects receiving the command. The default implementation returns `nil`.

You need to create a subclass of `NSScriptCommand` only if you need to provide a default implementation of a command.

## See Also

### Executing the command

func execute() -> Any?

Executes the command if it is valid and returns the result, if any.

