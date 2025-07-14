

- Foundation
- Process
-  terminationReason 

Instance Property

# terminationReason

The reason the system terminated the task.

macOS 10.6+

``` source
var terminationReason: Process.TerminationReason { get }
```

## Return Value

The termination status. The possible values are described in Process.TerminationReason.

## See Also

### Querying the State

var isRunning: Bool

A status that indicates whether the receiver is still running.

var terminationStatus: Int32

The exit status the receiver’s executable returns.

