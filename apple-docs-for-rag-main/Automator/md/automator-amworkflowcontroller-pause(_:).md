

- Automator
- AMWorkflowController
-  pause(\_:) 

Instance Method

# pause(\_:)

Pauses a workflow that’s running.

Mac Catalyst 14.0+macOS 10.4+

``` source
@IBAction @MainActor
func pause(_ sender: Any)
```

## Parameters 

`sender`  

Object that initiated the pause action.

## See Also

### Controlling the Workflow

func reset(Any)

Stops a workflow, clears any action results, and resets the workflow back to an un-run state.

func run(Any)

Runs the associated workflow, after first clearing any results stored by its actions during any previous run.

func step(Any)

In a paused workflow, runs the next action in the workflow and then pauses again.

func stop(Any)

Stops the associated workflow.

