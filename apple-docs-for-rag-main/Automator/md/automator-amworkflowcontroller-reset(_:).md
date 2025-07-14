

- Automator
- AMWorkflowController
-  reset(\_:) 

Instance Method

# reset(\_:)

Stops a workflow, clears any action results, and resets the workflow back to an un-run state.

Mac Catalyst 14.0+macOS 10.4+

``` source
@IBAction @MainActor
func reset(_ sender: Any)
```

## Parameters 

`sender`  

Object that initiated the reset action.

## See Also

### Controlling the Workflow

func pause(Any)

Pauses a workflow that’s running.

func run(Any)

Runs the associated workflow, after first clearing any results stored by its actions during any previous run.

func step(Any)

In a paused workflow, runs the next action in the workflow and then pauses again.

func stop(Any)

Stops the associated workflow.

