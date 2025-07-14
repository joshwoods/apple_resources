

- Foundation
- NSAppleScript
-  executeAppleEvent(\_:error:) 

Instance Method

# executeAppleEvent(\_:error:)

Executes an Apple event in the context of the receiver, as a means of allowing the application to invoke a handler in the script.

Mac Catalyst 13.0+macOS 10.0+

``` source
func executeAppleEvent(
    _ event: NSAppleEventDescriptor,
    error errorInfo: AutoreleasingUnsafeMutablePointer?
) -> NSAppleEventDescriptor
```

## Parameters 

`event`  

The Apple event to execute.

`errorInfo`  

On return, if an error occurs, a pointer to an error information dictionary.

## Return Value

The result of executing the event, or `nil` if an error occurs.

## Discussion

Compiles the receiver before executing it if it is not already compiled.

Important

You cannot use this method to send Apple events to other applications.

## See Also

### Compiling and Executing a Script

func compileAndReturnError(AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) -> Bool

Compiles the receiver, if it is not already compiled.

func executeAndReturnError(AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) -> NSAppleEventDescriptor

Executes the receiver, compiling it first if it is not already compiled.

