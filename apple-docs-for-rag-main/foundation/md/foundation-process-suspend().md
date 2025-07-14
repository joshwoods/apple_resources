

- Foundation
- Process
-  suspend() 

Instance Method

# suspend()

Suspends execution of the receiver task.

Mac Catalyst 13.0+macOS 10.0+

``` source
func suspend() -> Bool
```

## Return Value

true if the receiver was successfully suspended, false otherwise.

## Discussion

Multiple suspend() messages can be sent, but they must be balanced with an equal number of resume() messages before the task resumes execution.

## See Also

### Running and Stopping

func run() throws

Runs the process with the current environment.

func interrupt()

Sends an interrupt signal to the receiver and all of its subtasks.

func resume() -> Bool

Resumes execution of a suspended task.

func terminate()

Sends a terminate signal to the receiver and all of its subtasks.

func waitUntilExit()

Blocks the process until the receiver is finished.

