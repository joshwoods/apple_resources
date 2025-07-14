

- Automator
- AMAction
-  willFinishRunning() 

Instance Method

# willFinishRunning()

Provides an opportunity for an action to perform cleanup operations, such as closing windows and deallocating memory.

Mac Catalyst 14.0+macOS 10.5+

``` source
func willFinishRunning()
```

## Discussion

Overridde this method in actions that need to make asynchronous calls. Automator invokes this method when the action is about to complete its run phase.

## See Also

### Controlling the Action

func run(withInput: Any?) throws -> Any

Requests the action to perform its task using the specified input.

func runAsynchronously(withInput: Any?)

Causes Automator to wait for notification that the action has completed execution, which allows the action to perform an asynchronous operation.

func finishRunningWithError((any Error)?)

Causes the action to stop running and return an error, which, in turn, causes the workflow to stop.

func stop()

Stops the action from running.

func reset()

Resets the action to its initial state.

