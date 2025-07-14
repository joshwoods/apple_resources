

- Foundation
- NSScriptCommand
-  suspendExecution() 

Instance Method

# suspendExecution()

Suspends the execution of the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func suspendExecution()
```

## Discussion

Suspends the execution of the receiver only if the receiver is being executed in the current thread by Cocoa scripting’s built-in Apple event handling (that is, the receiver would be returned by `[NSScriptCommand currentCommand]`)—otherwise, does nothing. A matching invocation of resumeExecution(withResult:) must be made.

Important

The script command handler that is being executed when this method is invoked must return before the subsequent invocation of resumeExecution(withResult:). That is, it is not valid to suspend a command’s execution and then resume it immediately.

Another command can execute while a command is suspended.

## See Also

### Suspending and resuming commands

func resumeExecution(withResult: Any?)

If a successful, unmatched, invocation of suspendExecution() has been made, resume the execution of the command.

