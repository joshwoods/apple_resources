

- Foundation
- NSScriptCommand
-  resumeExecution(withResult:) 

Instance Method

# resumeExecution(withResult:)

If a successful, unmatched, invocation of suspendExecution() has been made, resume the execution of the command.

Mac Catalyst 13.0+macOS 10.0+

``` source
func resumeExecution(withResult result: Any?)
```

## Discussion

Resumes the execution of the command if a successful, unmatched, invocation of suspendExecution() has been made—otherwise, does nothing. The value for `result` is dependent on the segment of command execution that was suspended:

- If suspendExecution() was invoked from within a command handler of one of the command’s receivers, `result` is considered to be the return value of the handler. Unless the command has received a scriptErrorNumber message with a nonzero error number, execution of the command will continue and the command handlers of other receivers will be invoked.

- If suspendExecution() was invoked from within an override of performDefaultImplementation() the result is treated as if it were the return value of the invocation of performDefaultImplementation().

resumeExecution(withResult:) may be invoked in any thread, not just the one in which the corresponding invocation of suspendExecution() occurred.

Important

The script command handler that is being executed when suspendExecution() is invoked must return before you invoke resumeExecution(withResult:). That is, it is not valid to suspend a command’s execution and then resume it immediately.

## See Also

### Suspending and resuming commands

func suspendExecution()

Suspends the execution of the receiver.

