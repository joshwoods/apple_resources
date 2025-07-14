

- Foundation
- NSScriptCommandDescription
-  appleEventClassCode 

Instance Property

# appleEventClassCode

Returns the four-character code for the Apple event class of the receiver’s command.

Mac Catalyst 13.0+macOS 10.0+

``` source
var appleEventClassCode: FourCharCode { get }
```

## Return Value

The Apple event code associated with the receiver’s command. This is the primary code used to identify the command in Apple events.

## Discussion

In an Apple event that specifies a script command, two four character codes—the event class and event ID—together identify the command. You use this method to obtain the event class. You use appleEventCode to obtain the event ID.

For example, commands in AppleScript’s Core suite, such as `clone`, `count`, and `create`, have an event class code of `'core'`. This code and the event ID code returned by `appleEventCode` together specify the necessary information for identifying and dispatching an Apple event.

## See Also

### Getting Basic Information About the Command

var appleEventCode: FourCharCode

Returns the four-character code for the Apple event ID of the receiver’s command.

var commandClassName: String

Returns the name of the class that will be instantiated to handle the command.

var commandName: String

Returns the name of the command.

var suiteName: String

Returns the name of the suite that contains the command described by the receiver.

