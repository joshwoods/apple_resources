

- Automator
- AMWorkflow
-  run(at:withInput:) 

Type Method

# run(at:withInput:)

Loads and runs the specified workflow file.

Mac Catalyst 14.0+macOS 10.4+

``` source
class func run(
    at fileURL: URL,
    withInput input: Any?
) throws -> Any
```

## Parameters 

`fileURL`  

A URL that specifies the location of a workflow file.

`input`  

The input for the first action in the workflow. Pass `nil` if the first action doesn’t need input.

## Return Value

This method returns `nil` on error, or if the action completes successfully without producing output. The error argument must be examined to determine which scenario occurred. Otherwise, this method returns the output of the last action in the workflow. Your application may need to convert the data to a desired type.

## Discussion

Use this method to run a workflow without the overhead of performing a separate allocation, setting up a workflow controller, and so on. In situations where you need greater control, such as the ability to start and stop the workflow, use an instance of the AMWorkflowController class instead.

The workflow is run in a separate process so that any actions it contains are executed in a separate memory space. This helps to insulate the app from crashes, memory leaks, or exceptions that might occur from running the actions in the workflow.

