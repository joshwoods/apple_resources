

- Foundation
- Process
-  run() 

Instance Method

# run()

Runs the process with the current environment.

macOS 10.13+

``` source
func run() throws
```

## See Also

### Running and Stopping

func interrupt()

Sends an interrupt signal to the receiver and all of its subtasks.

func resume() -> Bool

Resumes execution of a suspended task.

func suspend() -> Bool

Suspends execution of the receiver task.

func terminate()

Sends a terminate signal to the receiver and all of its subtasks.

func waitUntilExit()

Blocks the process until the receiver is finished.

