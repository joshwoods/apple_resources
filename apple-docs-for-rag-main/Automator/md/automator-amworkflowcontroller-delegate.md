

- Automator
- AMWorkflowController
-  delegate 

Instance Property

# delegate

The controller’s delegate.

Mac Catalyst 14.0+macOS 10.4+

``` source
weak var delegate: (any AMWorkflowControllerDelegate)? { get set }
```

## Return Value

The controller’s delegate.

## Discussion

This object receives updates on the progress and state of the workflow controller.

## See Also

### Accessing the Delegate

protocol AMWorkflowControllerDelegate

A set of optional methods that a delegate of a workflow controller implements.

