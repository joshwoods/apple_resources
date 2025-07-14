

- Automator
- AMAction
-  reset() 

Instance Method

# reset()

Resets the action to its initial state.

Mac Catalyst 14.0+macOS 10.4+

``` source
func reset()
```

## Discussion

Resetting causes the action to release its output generated from the current execution of the workflow.

## See Also

### Controlling the Action

func run(withInput: Any?) throws -> Any

Requests the action to perform its task using the specified input.

func runAsynchronously(withInput: Any?)

Causes Automator to wait for notification that the action has completed execution, which allows the action to perform an asynchronous operation.

func finishRunningWithError((any Error)?)

Causes the action to stop running and return an error, which, in turn, causes the workflow to stop.

func willFinishRunning()

Provides an opportunity for an action to perform cleanup operations, such as closing windows and deallocating memory.

func stop()

Stops the action from running.

