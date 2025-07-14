

- Foundation
- NSScriptCommandDescription
-  commandClassName 

Instance Property

# commandClassName

Returns the name of the class that will be instantiated to handle the command.

Mac Catalyst 13.0+macOS 10.0+

``` source
var commandClassName: String { get }
```

## Return Value

The Objective-C class name (for example, `"NSGetCommand"`). This is always NSScriptCommand or a subclass.

## See Also

### Getting Basic Information About the Command

var appleEventClassCode: FourCharCode

Returns the four-character code for the Apple event class of the receiver’s command.

var appleEventCode: FourCharCode

Returns the four-character code for the Apple event ID of the receiver’s command.

var commandName: String

Returns the name of the command.

var suiteName: String

Returns the name of the suite that contains the command described by the receiver.

