

- Foundation
- NSScriptCommand
-  scriptErrorString 

Instance Property

# scriptErrorString

Sets a script error string that is associated with execution of the command.

Mac Catalyst 13.0+macOS 10.0+

``` source
var scriptErrorString: String? { get set }
```

## Parameters 

`errorString`  

A string that describes an error.

## Discussion

If you override performDefaultImplementation() and an error occurs, you should call this method to supply a string that provides a useful explanation. In fact, any script handler should call this method when an error occurs.

Calling this method alone does not cause an error message to be displayed—you must also call scriptErrorNumber to supply an error number.

## See Also

### Handling script execution errors

var scriptErrorExpectedTypeDescriptor: NSAppleEventDescriptor?

Sets a descriptor for the expected type that will be put in the reply Apple event if the sender requested a reply, execution of the receiver completes, and an error number was set.

var scriptErrorNumber: Int

Sets a script error number that is associated with the execution of the command and is returned in the reply Apple event, if a reply was requested by the sender.

var scriptErrorOffendingObjectDescriptor: NSAppleEventDescriptor?

Sets a descriptor for an object that will be put in the reply Apple event if the sender requested a reply, execution of the receiver completes, and an error number was set.

