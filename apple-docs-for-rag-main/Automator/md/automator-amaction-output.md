

- Automator
- AMAction
-  output 

Instance Property

# output

The action’s output.

Mac Catalyst 14.0+macOS 10.5+

``` source
var output: Any? { get set }
```

## Return Value

The receiving action’s output, or `nil` if called before the action is run.

## Discussion

`nil` if called before the action is run.

This method is used in conjunction with the AMWorkflow class, which allows access to the actions in a workflow. Within a workflow, for example, you might iteratively inspect the output of each action. Or, on completion of a workflow, you might examine the output of the last action, to determine the output of the workflow.

This parameter can also be used when running an action asynchronously. Call `setOutput` to specify the output the action produces.

## See Also

### Getting Action Information

var name: String

The name of the action.

var progressValue: CGFloat

A float value between 0 and 1, which indicates how far along the action is while processing.

var ignoresInput: Bool

A Boolean value that indicates whether the action acts upon its input or the input is ignored.

var selectedInputType: String?

The type of input, in UTI format, of the input received by the action.

var selectedOutputType: String?

The type of output, in UTI format, of the output to be produced by the action.

var isStopped: Bool

A Boolean value that indicates whether the user clicked the stop button on the parent workflow.

