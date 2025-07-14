

- Foundation
- NSScriptCommandDescription
-  appleEventCode 

Instance Property

# appleEventCode

Returns the four-character code for the Apple event ID of the receiver’s command.

Mac Catalyst 13.0+macOS 10.0+

``` source
var appleEventCode: FourCharCode { get }
```

## Return Value

The code for the event ID of the receiver’s command.

## Discussion

This value of the event ID returned by this method, together with the event class code returned by appleEventClassCode, specifies the necessary information for identifying and dispatching an Apple event.

## See Also

### Related Documentation

var appleEventCodeForReturnType: FourCharCode

Returns the Apple event code that identifies the command’s return type.

func appleEventCodeForArgument(withName: String) -> FourCharCode

Returns the Apple event code for the specified command argument of the receiver.

### Getting Basic Information About the Command

var appleEventClassCode: FourCharCode

Returns the four-character code for the Apple event class of the receiver’s command.

var commandClassName: String

Returns the name of the class that will be instantiated to handle the command.

var commandName: String

Returns the name of the command.

var suiteName: String

Returns the name of the suite that contains the command described by the receiver.

