

- Automator
- AMWorkflowController
-  canRun 

Instance Property

# canRun

A Boolean value that indicates whether the controller’s workflow is able to run.

Mac Catalyst 14.0+macOS 10.4+

``` source
var canRun: Bool { get }
```

## Return Value

true if the controller’s workflow is able to run; false otherwise.

## Discussion

You might use this method to determine when to enable a “Run” button or other UI element you use to run the workflow.

## See Also

### Getting Workflow Information

var isPaused: Bool

A Boolean value that indicates whether the controller’s workflow is currently paused.

var isRunning: Bool

A Boolean value that indicates whether the controller’s workflow is currently running.

