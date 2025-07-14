

- Foundation
- NSScriptCommandDescription
-  typeForArgument(withName:) 

Instance Method

# typeForArgument(withName:)

Returns the type of the command argument identified by the specified key.

Mac Catalyst 13.0+macOS 10.0+

``` source
func typeForArgument(withName argumentName: String) -> String?
```

## Parameters 

`argumentName`  

Argument name (used as a key) that identifies the command argument to examine.

## Return Value

The type of the specified command argument. Returns `nil` if there is no such argument.

## See Also

### Getting Command Argument Information

func appleEventCodeForArgument(withName: String) -> FourCharCode

Returns the Apple event code for the specified command argument of the receiver.

var argumentNames: [String]

Returns the names (or keys) for all arguments of the receiver’s command.

func isOptionalArgument(withName: String) -> Bool

Returns a Boolean value that indicates whether the command argument identified by the specified argument key is an optional argument.

