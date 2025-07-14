

- Automator
- AMAction
-  run(withInput:) 

Instance Method

# run(withInput:)

Requests the action to perform its task using the specified input.

Mac Catalyst 14.0+macOS 10.7+

``` source
func run(withInput input: Any?) throws -> Any
```

## Parameters 

`input`  

The input for the receiving action. Should contain one or more objects compatible with one of the types specified in the action’s selectedInputType property.

## Return Value

An NSArray object that contains one or more objects of a data type compatible with a type specified in the receiving action’s `AMProvides` property. If the action doesn’t modify the data passed in `input`, it should return it unchanged. If the action doesn’t have any data to provide, it should return an empty NSArray object.

## Discussion

This method is intended to be overridden.

The input and output objects for actions are usually instances of NSArray. If the action encounters problems, it should return by indirection an NSError object that describes the error.

## See Also

### Controlling the Action

func runAsynchronously(withInput: Any?)

Causes Automator to wait for notification that the action has completed execution, which allows the action to perform an asynchronous operation.

func finishRunningWithError((any Error)?)

Causes the action to stop running and return an error, which, in turn, causes the workflow to stop.

func willFinishRunning()

Provides an opportunity for an action to perform cleanup operations, such as closing windows and deallocating memory.

func stop()

Stops the action from running.

func reset()

Resets the action to its initial state.

