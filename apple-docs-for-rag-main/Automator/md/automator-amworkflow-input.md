

- Automator
- AMWorkflow
-  input 

Instance Property

# input

The input data that is passed to the first action in the workflow.

Mac Catalyst 14.0+macOS 10.4+

``` source
var input: Any? { get set }
```

## Return Value

The input for the first action in the workflow. Should be a data type the action can use, or a type that can be converted to one the action can use. Use `setInput:` to set the input data for the workflow.

## See Also

### Working with the Workflow’s Input and Output

var output: Any?

The output data that is provided by the last action in the workflow.

