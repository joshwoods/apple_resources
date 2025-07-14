

- Automator
- AMWorkflowController
-  isRunning 

Instance Property

# isRunning

A Boolean value that indicates whether the controller’s workflow is currently running.

Mac Catalyst 14.0+macOS 10.4+

``` source
var isRunning: Bool { get }
```

## Discussion

true if the controller’s workflow is currently running; false otherwise. Use `isRunning:` to determine whether the receiver’s workflow is currently running.

## See Also

### Getting Workflow Information

var canRun: Bool

A Boolean value that indicates whether the controller’s workflow is able to run.

var isPaused: Bool

A Boolean value that indicates whether the controller’s workflow is currently paused.

