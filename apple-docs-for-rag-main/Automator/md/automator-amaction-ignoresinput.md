

- Automator
- AMAction
-  ignoresInput 

Instance Property

# ignoresInput

A Boolean value that indicates whether the action acts upon its input or the input is ignored.

Mac Catalyst 14.0+macOS 10.5+

``` source
var ignoresInput: Bool { get }
```

## Discussion

true if the action acts upon its input, otherwise false.

Many actions act upon their input, but an action may merely pass on its input or, rarely, ignore it.

## See Also

### Getting Action Information

var name: String

The name of the action.

var progressValue: CGFloat

A float value between 0 and 1, which indicates how far along the action is while processing.

var output: Any?

The action’s output.

var selectedInputType: String?

The type of input, in UTI format, of the input received by the action.

var selectedOutputType: String?

The type of output, in UTI format, of the output to be produced by the action.

var isStopped: Bool

A Boolean value that indicates whether the user clicked the stop button on the parent workflow.

