

- Automator
- AMWorkflowControllerDelegate
-  workflowController(\_:didError:) 

Instance Method

# workflowController(\_:didError:)

Notifies the delegate when the workflow encounters an error.

Mac Catalyst 14.0+macOS 10.4+

``` source
optional func workflowController(
    _ controller: AMWorkflowController,
    didError error: any Error
)
```

## Parameters 

`controller`  

The controller object sending the message.

`error`  

If a workflow error occurs, upon return contains an instance of NSError that describes the problem.

