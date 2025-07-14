

- Foundation
- Process
-  isRunning 

Instance Property

# isRunning

A status that indicates whether the receiver is still running.

Mac Catalyst 13.0+macOS 10.0+

``` source
var isRunning: Bool { get }
```

## Return Value

true if the receiver is still running, otherwise false. false means either the receiver could not run or it has terminated.

## See Also

### Related Documentation

func waitUntilExit()

Blocks the process until the receiver is finished.

func launch()

Launches the task represented by the receiver.

Deprecated

func terminate()

Sends a terminate signal to the receiver and all of its subtasks.

### Querying the State

var terminationStatus: Int32

The exit status the receiver’s executable returns.

var terminationReason: Process.TerminationReason

The reason the system terminated the task.

