

- Automator
- AMWorkflowControllerDelegate
-  workflowControllerWillStop(\_:) 

Instance Method

# workflowControllerWillStop(\_:)

Tells the delegate that the workflow controller object is about to stop.

Mac Catalyst 14.0+macOS 10.4+

``` source
optional func workflowControllerWillStop(_ controller: AMWorkflowController)
```

## Parameters 

`controller`  

The workflow controller object to stop.

## See Also

### Stopping

func workflowControllerDidStop(AMWorkflowController)

Tells the delegate that the workflow controller object has stopped.

