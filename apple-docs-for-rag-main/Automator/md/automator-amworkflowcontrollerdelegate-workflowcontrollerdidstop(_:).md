

- Automator
- AMWorkflowControllerDelegate
-  workflowControllerDidStop(\_:) 

Instance Method

# workflowControllerDidStop(\_:)

Tells the delegate that the workflow controller object has stopped.

Mac Catalyst 14.0+macOS 10.4+

``` source
optional func workflowControllerDidStop(_ controller: AMWorkflowController)
```

## Parameters 

`controller`  

The workflow controller object that stopped.

## See Also

### Stopping

func workflowControllerWillStop(AMWorkflowController)

Tells the delegate that the workflow controller object is about to stop.

