

- Automator
- AMWorkflowController
-  run(\_:) 

Instance Method

# run(\_:)

Runs the associated workflow, after first clearing any results stored by its actions during any previous run.

Mac Catalyst 14.0+macOS 10.4+

``` source
@IBAction @MainActor
func run(_ sender: Any)
```

## Parameters 

`sender`  

Object that initiated the run action.

## See Also

### Controlling the Workflow

func pause(Any)

Pauses a workflow that’s running.

func reset(Any)

Stops a workflow, clears any action results, and resets the workflow back to an un-run state.

func step(Any)

In a paused workflow, runs the next action in the workflow and then pauses again.

func stop(Any)

Stops the associated workflow.

