

- Automator
- AMAction
-  isStopped 

Instance Property

# isStopped

A Boolean value that indicates whether the user clicked the stop button on the parent workflow.

Mac Catalyst 14.0+macOS 10.4+

``` source
var isStopped: Bool { get }
```

## Discussion

This value is true if the user clicked the stop button, or false if the workflow is still running. This property should be referenced during lengthy action processes, such as a loop, in order to determine whether to exit the operation and stop the action.

## See Also

### Getting Action Information

var name: String

The name of the action.

var progressValue: CGFloat

A float value between 0 and 1, which indicates how far along the action is while processing.

var ignoresInput: Bool

A Boolean value that indicates whether the action acts upon its input or the input is ignored.

var output: Any?

The action’s output.

var selectedInputType: String?

The type of input, in UTI format, of the input received by the action.

var selectedOutputType: String?

The type of output, in UTI format, of the output to be produced by the action.

