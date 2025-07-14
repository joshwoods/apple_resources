

- Automator
- AMAction
-  name 

Instance Property

# name

The name of the action.

Mac Catalyst 14.0+macOS 10.5+

``` source
var name: String { get }
```

## See Also

### Getting Action Information

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

var isStopped: Bool

A Boolean value that indicates whether the user clicked the stop button on the parent workflow.

