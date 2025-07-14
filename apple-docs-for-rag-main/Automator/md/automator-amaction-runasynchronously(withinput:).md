

- Automator
- AMAction
-  runAsynchronously(withInput:) 

Instance Method

# runAsynchronously(withInput:)

Causes Automator to wait for notification that the action has completed execution, which allows the action to perform an asynchronous operation.

Mac Catalyst 14.0+macOS 10.5+

``` source
func runAsynchronously(withInput input: Any?)
```

## Parameters 

`input`  

The input for the action. Should contain one or more objects compatible with one of the types specified in the action’s selectedInputType property.

## Discussion

Override this method in actions that need to make asynchronous calls. After runAsynchronously(withInput:) is invoked, Automator doesn’t continue until the action invokes finishRunningWithError(_:). In your override of this method, you can make an asynchronous call, wait to be notified of its completion, then invoke finishRunningWithError(_:) to signal to Automator that the action has completed.

Warning

Failure to invoke finishRunningWithError(_:) can cause a workflow to stall indefinitely.

For actions that don’t need to make asynchronous calls, use runWithInput:fromAction:error: instead.

## See Also

### Controlling the Action

func run(withInput: Any?) throws -> Any

Requests the action to perform its task using the specified input.

func finishRunningWithError((any Error)?)

Causes the action to stop running and return an error, which, in turn, causes the workflow to stop.

func willFinishRunning()

Provides an opportunity for an action to perform cleanup operations, such as closing windows and deallocating memory.

func stop()

Stops the action from running.

func reset()

Resets the action to its initial state.

