

- Automator
- AMWorkspace
-  runWorkflow(atPath:withInput:) 

Instance Method

# runWorkflow(atPath:withInput:)

Loads and runs the specified workflow file.

Mac Catalyst 14.0+macOS 10.4+

``` source
func runWorkflow(
    atPath path: String!,
    withInput input: Any!
) throws -> Any
```

## Parameters 

`path`  

A path that specifies the location of the workflow file.

`input`  

The input for the first action in the workflow. Pass `nil` if the first action doesn’t need input.

## Return Value

`nil` if an error occurs or if the action completes successfully without producing output; otherwise, the output of the last action in the workflow.

