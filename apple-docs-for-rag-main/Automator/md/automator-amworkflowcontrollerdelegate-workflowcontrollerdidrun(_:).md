

- Automator
- AMWorkflowControllerDelegate
-  workflowControllerDidRun(\_:) 

Instance Method

# workflowControllerDidRun(\_:)

Notifies the delegate when the workflow controller object finishes running.

Mac Catalyst 14.0+macOS 10.4+

``` source
optional func workflowControllerDidRun(_ controller: AMWorkflowController)
```

## Parameters 

`controller`  

The workflow controller object that finished running.

## See Also

### Running

func workflowController(AMWorkflowController, didRun: AMAction)

Notifies the delegate when the specified action finishes running.

