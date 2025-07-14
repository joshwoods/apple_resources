

- Foundation
- Process
-  terminationStatus 

Instance Property

# terminationStatus

The exit status the receiver’s executable returns.

Mac Catalyst 13.0+macOS 10.0+

``` source
var terminationStatus: Int32 { get }
```

## Return Value

The exit status returned by the receiver’s executable.

## Discussion

Each task defines and documents how your app should interpret the return value. For example, many commands return 0 if they complete successfully or an error code if they don’t. You’ll need to look at the documentation for that task to learn what values it returns under what circumstances.

This method raises an `NSInvalidArgumentException` if the receiver is still running. Verify that the receiver isn’t running before you use it.

- Swift
- Objective-C

```
let task: NSTask = // Create and initialize a task
if !task.isRunning {
    let status = task.terminationStatus
    if status == 0 {
        print("Task succeeded.")
    } else {
        print("Task failed.")
    }
}
```

```
NSTask *task = // Create and initialize a task
if (![task isRunning]) {
    int status = [task terminationStatus];
    if (status == 0) {
        NSLog(@"Task succeeded.");
    } else {
        NSLog(@"Task failed.");
    }
}
```

## See Also

### Related Documentation

func waitUntilExit()

Blocks the process until the receiver is finished.

func terminate()

Sends a terminate signal to the receiver and all of its subtasks.

### Querying the State

var isRunning: Bool

A status that indicates whether the receiver is still running.

var terminationReason: Process.TerminationReason

The reason the system terminated the task.

