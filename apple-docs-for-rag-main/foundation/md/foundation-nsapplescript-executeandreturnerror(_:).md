

- Foundation
- NSAppleScript
-  executeAndReturnError(\_:) 

Instance Method

# executeAndReturnError(\_:)

Executes the receiver, compiling it first if it is not already compiled.

Mac Catalyst 13.0+macOS 10.0+

``` source
func executeAndReturnError(_ errorInfo: AutoreleasingUnsafeMutablePointer?) -> NSAppleEventDescriptor
```

## Parameters 

`errorInfo`  

On return, if an error occurs, a pointer to an error information dictionary.

## Return Value

The result of executing the event, or `nil` if an error occurs.

## Discussion

Any changes to property values caused by executing the script do not persist.

## See Also

### Compiling and Executing a Script

func compileAndReturnError(AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) -> Bool

Compiles the receiver, if it is not already compiled.

func executeAppleEvent(NSAppleEventDescriptor, error: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) -> NSAppleEventDescriptor

Executes an Apple event in the context of the receiver, as a means of allowing the application to invoke a handler in the script.

