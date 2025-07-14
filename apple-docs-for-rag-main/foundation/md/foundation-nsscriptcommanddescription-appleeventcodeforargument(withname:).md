

- Foundation
- NSScriptCommandDescription
-  appleEventCodeForArgument(withName:) 

Instance Method

# appleEventCodeForArgument(withName:)

Returns the Apple event code for the specified command argument of the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func appleEventCodeForArgument(withName argumentName: String) -> FourCharCode
```

## Parameters 

`argumentName`  

The argument name (used as a key) for which to obtain the corresponding Apple event code.

## Return Value

The code for the specified argument.

## See Also

### Getting Command Argument Information

var argumentNames: [String]

Returns the names (or keys) for all arguments of the receiver’s command.

func isOptionalArgument(withName: String) -> Bool

Returns a Boolean value that indicates whether the command argument identified by the specified argument key is an optional argument.

func typeForArgument(withName: String) -> String?

Returns the type of the command argument identified by the specified key.

