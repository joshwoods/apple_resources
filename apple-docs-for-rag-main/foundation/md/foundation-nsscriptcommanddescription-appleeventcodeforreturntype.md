

- Foundation
- NSScriptCommandDescription
-  appleEventCodeForReturnType 

Instance Property

# appleEventCodeForReturnType

Returns the Apple event code that identifies the command’s return type.

Mac Catalyst 13.0+macOS 10.0+

``` source
var appleEventCodeForReturnType: FourCharCode { get }
```

## Return Value

The event code for the command’s return type.

## See Also

### Related Documentation

func appleEventCodeForArgument(withName: String) -> FourCharCode

Returns the Apple event code for the specified command argument of the receiver.

### Getting Command Return-Type Information

var returnType: String?

Returns the return type of the command.

