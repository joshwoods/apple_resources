

- Foundation
- NSAppleScript
-  compileAndReturnError(\_:) 

Instance Method

# compileAndReturnError(\_:)

Compiles the receiver, if it is not already compiled.

Mac Catalyst 13.0+macOS 10.0+

``` source
func compileAndReturnError(_ errorInfo: AutoreleasingUnsafeMutablePointer?) -> Bool
```

## Parameters 

`errorInfo`  

On return, if an error occurs, a pointer to an error information dictionary.

## Return Value

true for success or if the script was already compiled, false otherwise.

## See Also

### Compiling and Executing a Script

func executeAndReturnError(AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) -> NSAppleEventDescriptor

Executes the receiver, compiling it first if it is not already compiled.

func executeAppleEvent(NSAppleEventDescriptor, error: AutoreleasingUnsafeMutablePointer&lt;NSDictionary?>?) -> NSAppleEventDescriptor

Executes an Apple event in the context of the receiver, as a means of allowing the application to invoke a handler in the script.

