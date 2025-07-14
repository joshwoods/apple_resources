

- Foundation
- Process
-  resume() 

Instance Method

# resume()

Resumes execution of a suspended task.

Mac Catalyst 13.0+macOS 10.0+

``` source
func resume() -> Bool
```

## Return Value

true if the receiver was able to resume execution, false otherwise.

## Discussion

If the system sent multiple suspend() messages to the receiver, an equal number of resume() messages must be sent before the task resumes execution.

## See Also

### Running and Stopping

func run() throws

Runs the process with the current environment.

func interrupt()

Sends an interrupt signal to the receiver and all of its subtasks.

func suspend() -> Bool

Suspends execution of the receiver task.

func terminate()

Sends a terminate signal to the receiver and all of its subtasks.

func waitUntilExit()

Blocks the process until the receiver is finished.

