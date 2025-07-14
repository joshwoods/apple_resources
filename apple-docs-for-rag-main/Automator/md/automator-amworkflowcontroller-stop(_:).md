

- Automator
- AMWorkflowController
-  stop(\_:) 

Instance Method

# stop(\_:)

Stops the associated workflow.

Mac Catalyst 14.0+macOS 10.4+

``` source
@IBAction @MainActor
func stop(_ sender: Any)
```

## Parameters 

`sender`  

Object that initiated the stop action.

## See Also

### Controlling the Workflow

func pause(Any)

Pauses a workflow that’s running.

func reset(Any)

Stops a workflow, clears any action results, and resets the workflow back to an un-run state.

func run(Any)

Runs the associated workflow, after first clearing any results stored by its actions during any previous run.

func step(Any)

In a paused workflow, runs the next action in the workflow and then pauses again.

