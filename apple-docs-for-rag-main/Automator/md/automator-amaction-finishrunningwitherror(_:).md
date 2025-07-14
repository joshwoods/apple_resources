

- Automator
- AMAction
-  finishRunningWithError(\_:) 

Instance Method

# finishRunningWithError(\_:)

Causes the action to stop running and return an error, which, in turn, causes the workflow to stop.

Mac Catalyst 14.0+macOS 10.7+

``` source
func finishRunningWithError(_ error: (any Error)?)
```

## Parameters 

`error`  

The error to be returned to Automator.

## Discussion

Call this method on any action that overrides runAsynchronously(withInput:) in order to make asynchronous calls. When finishRunningWithError(_:) is invoked, it immediately calls willFinishRunning().

## See Also

### Controlling the Action

func run(withInput: Any?) throws -> Any

Requests the action to perform its task using the specified input.

func runAsynchronously(withInput: Any?)

Causes Automator to wait for notification that the action has completed execution, which allows the action to perform an asynchronous operation.

func willFinishRunning()

Provides an opportunity for an action to perform cleanup operations, such as closing windows and deallocating memory.

func stop()

Stops the action from running.

func reset()

Resets the action to its initial state.

