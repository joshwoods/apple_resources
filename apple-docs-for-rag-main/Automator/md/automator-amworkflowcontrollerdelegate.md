

- Automator
-  AMWorkflowControllerDelegate 

Protocol

# AMWorkflowControllerDelegate

A set of optional methods that a delegate of a workflow controller implements.

Mac Catalyst 14.0+macOS 10.4+

``` source
protocol AMWorkflowControllerDelegate : NSObjectProtocol
```

## Topics

### Preparing to Run

func workflowController(AMWorkflowController, willRun: AMAction)

Notifies the delegate when the specified action is about to run.

func workflowControllerWillRun(AMWorkflowController)

Notifies the delegate when the workflow controller object is about to run.

### Running

func workflowController(AMWorkflowController, didRun: AMAction)

Notifies the delegate when the specified action finishes running.

func workflowControllerDidRun(AMWorkflowController)

Notifies the delegate when the workflow controller object finishes running.

### Stopping

func workflowControllerWillStop(AMWorkflowController)

Tells the delegate that the workflow controller object is about to stop.

func workflowControllerDidStop(AMWorkflowController)

Tells the delegate that the workflow controller object has stopped.

### Handling Errors

func workflowController(AMWorkflowController, didError: any Error)

Notifies the delegate when the workflow encounters an error.

### Deprecated

optional func workflowController(_ controller: AMWorkflowController, willRun action: AMAction)

Notifies the delegate when the specified action is about to run.

optional func workflowControllerWillRun(_ controller: AMWorkflowController)

Notifies the delegate when the workflow controller object is about to run.

optional func workflowController(_ controller: AMWorkflowController, didRun action: AMAction)

Notifies the delegate when the specified action finishes running.

optional func workflowControllerDidRun(_ controller: AMWorkflowController)

Notifies the delegate when the workflow controller object finishes running.

optional func workflowControllerWillStop(_ controller: AMWorkflowController)

Tells the delegate that the workflow controller object is about to stop.

optional func workflowControllerDidStop(_ controller: AMWorkflowController)

Tells the delegate that the workflow controller object has stopped.

optional func workflowController(_ controller: AMWorkflowController, didError error: any Error)

Notifies the delegate when the workflow encounters an error.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Accessing the Delegate

var delegate: (any AMWorkflowControllerDelegate)?

The controller’s delegate.

