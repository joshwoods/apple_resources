

- Foundation
- NSScriptCommandDescription
-  argumentNames 

Instance Property

# argumentNames

Returns the names (or keys) for all arguments of the receiver’s command.

Mac Catalyst 13.0+macOS 10.0+

``` source
var argumentNames: [String] { get }
```

## Return Value

The array of argument names. If there are no arguments for the command, returns an empty array.

## See Also

### Getting Command Argument Information

func appleEventCodeForArgument(withName: String) -> FourCharCode

Returns the Apple event code for the specified command argument of the receiver.

func isOptionalArgument(withName: String) -> Bool

Returns a Boolean value that indicates whether the command argument identified by the specified argument key is an optional argument.

func typeForArgument(withName: String) -> String?

Returns the type of the command argument identified by the specified key.

