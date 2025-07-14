

- Foundation
- Process
-  terminate() 

Instance Method

# terminate()

Sends a terminate signal to the receiver and all of its subtasks.

Mac Catalyst 13.0+macOS 10.0+

``` source
func terminate()
```

## Discussion

If the task terminates as a result, which is the default behavior, an didTerminateNotification gets sent to the default notification center. This method has no effect if the receiver was already launched and has already finished executing. If the receiver hasn’t been launched yet, this method raises an `NSInvalidArgumentException`.

It’s not always possible to terminate the receiver because it might be ignoring the terminate signal. The terminate() method sends `SIGTERM`.

## See Also

### Related Documentation

func launch()

Launches the task represented by the receiver.

Deprecated

class func launchedProcess(launchPath: String, arguments: [String]) -> Process

Creates and launches a task with a specified executable and arguments.

Deprecated

var terminationStatus: Int32

The exit status the receiver’s executable returns.

### Running and Stopping

func run() throws

Runs the process with the current environment.

func interrupt()

Sends an interrupt signal to the receiver and all of its subtasks.

func resume() -> Bool

Resumes execution of a suspended task.

func suspend() -> Bool

Suspends execution of the receiver task.

func waitUntilExit()

Blocks the process until the receiver is finished.

