

- Foundation
- Process
-  waitUntilExit() 

Instance Method

# waitUntilExit()

Blocks the process until the receiver is finished.

Mac Catalyst 13.0+macOS 10.0+

``` source
func waitUntilExit()
```

## Discussion

This method first checks to see if the receiver is still running using isRunning. Then it polls the current run loop using `NSDefaultRunLoopMode` until the task completes.

- Swift
- Objective-C

```
let task: NSTask = // Create and initialize a task
    task.launch()
task.waitUntilExit()
let status = task.terminationStatus

if status == 0 {
    print("Task succeeded.")
} else {
    print("Task failed.")
}
```

```
NSTask *task = // Create and initialize a task
[task launch];
[task waitUntilExit];
int status = [task terminationStatus];

if (status == 0) {
    NSLog(@"Task succeeded.");
} else {
    NSLog(@"Task failed.");
}
```

waitUntilExit() does not guarantee that the terminationHandler block has been fully executed before waitUntilExit() returns.

## See Also

### Related Documentation

func launch()

Launches the task represented by the receiver.

Deprecated

### Running and Stopping

func run() throws

Runs the process with the current environment.

func interrupt()

Sends an interrupt signal to the receiver and all of its subtasks.

func resume() -> Bool

Resumes execution of a suspended task.

func suspend() -> Bool

Suspends execution of the receiver task.

func terminate()

Sends a terminate signal to the receiver and all of its subtasks.

