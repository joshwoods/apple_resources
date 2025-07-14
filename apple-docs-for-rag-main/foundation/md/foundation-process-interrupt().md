

- Foundation
- Process
-  interrupt() 

Instance Method

# interrupt()

Sends an interrupt signal to the receiver and all of its subtasks.

Mac Catalyst 13.0+macOS 10.0+

``` source
func interrupt()
```

## Discussion

If the task terminates as a result, which is the default behavior, an didTerminateNotification gets sent to the default notification center. This method has no effect if the receiver was already launched and has already finished executing. If the system hasn’t launched the receiver, this method raises an `NSInvalidArgumentException`.

It isn’t always possible to interrupt the receiver because it might be ignoring the interrupt signal. The interrupt() method sends `SIGINT`.

## See Also

### Running and Stopping

func run() throws

Runs the process with the current environment.

func resume() -> Bool

Resumes execution of a suspended task.

func suspend() -> Bool

Suspends execution of the receiver task.

func terminate()

Sends a terminate signal to the receiver and all of its subtasks.

func waitUntilExit()

Blocks the process until the receiver is finished.

