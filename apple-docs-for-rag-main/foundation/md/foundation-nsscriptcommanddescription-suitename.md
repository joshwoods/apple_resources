

- Foundation
- NSScriptCommandDescription
-  suiteName 

Instance Property

# suiteName

Returns the name of the suite that contains the command described by the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var suiteName: String { get }
```

## Return Value

The receiver’s suite name. Within an application’s scriptability information, named suites contain related sets of information.

## See Also

### Getting Basic Information About the Command

var appleEventClassCode: FourCharCode

Returns the four-character code for the Apple event class of the receiver’s command.

var appleEventCode: FourCharCode

Returns the four-character code for the Apple event ID of the receiver’s command.

var commandClassName: String

Returns the name of the class that will be instantiated to handle the command.

var commandName: String

Returns the name of the command.

