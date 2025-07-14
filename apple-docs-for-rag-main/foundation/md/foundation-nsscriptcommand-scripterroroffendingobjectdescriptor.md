

- Foundation
- NSScriptCommand
-  scriptErrorOffendingObjectDescriptor 

Instance Property

# scriptErrorOffendingObjectDescriptor

Sets a descriptor for an object that will be put in the reply Apple event if the sender requested a reply, execution of the receiver completes, and an error number was set.

macOS 10.5+

``` source
var scriptErrorOffendingObjectDescriptor: NSAppleEventDescriptor? { get set }
```

## Parameters 

`errorOffendingObjectDescriptor`  

A descriptor that specifies an object that was responsible for an error.

## See Also

### Handling script execution errors

var scriptErrorExpectedTypeDescriptor: NSAppleEventDescriptor?

Sets a descriptor for the expected type that will be put in the reply Apple event if the sender requested a reply, execution of the receiver completes, and an error number was set.

var scriptErrorNumber: Int

Sets a script error number that is associated with the execution of the command and is returned in the reply Apple event, if a reply was requested by the sender.

var scriptErrorString: String?

Sets a script error string that is associated with execution of the command.

