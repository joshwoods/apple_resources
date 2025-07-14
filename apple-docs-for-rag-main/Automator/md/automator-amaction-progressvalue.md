

- Automator
- AMAction
-  progressValue 

Instance Property

# progressValue

A float value between 0 and 1, which indicates how far along the action is while processing.

Mac Catalyst 14.0+macOS 10.6+

``` source
var progressValue: CGFloat { get set }
```

## Discussion

Setting this value causes Automator’s action progress indicator (displayed as a workflow runs) to update in order to provide the user with an indication of progress.

## See Also

### Getting Action Information

var name: String

The name of the action.

var ignoresInput: Bool

A Boolean value that indicates whether the action acts upon its input or the input is ignored.

var output: Any?

The action’s output.

var selectedInputType: String?

The type of input, in UTI format, of the input received by the action.

var selectedOutputType: String?

The type of output, in UTI format, of the output to be produced by the action.

var isStopped: Bool

A Boolean value that indicates whether the user clicked the stop button on the parent workflow.

