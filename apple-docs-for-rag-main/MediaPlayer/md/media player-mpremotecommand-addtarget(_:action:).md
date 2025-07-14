

- Media Player
- MPRemoteCommand
-  addTarget(\_:action:) 

Instance Method

# addTarget(\_:action:)

Adds a target object to be called when an event is received.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
func addTarget(
    _ target: Any,
    action: Selector
)
```

## Parameters 

`target`  

The object to receive action messages sent by the receiver when the represented remote command is triggered. The value must not be `nil`.

`action`  

A selector identifying the method on the target to be called. The value must not be `NULL`.

The method to be called must have the following signature:

```
- (MPRemoteCommandHandlerStatus) handleCommand: (MPRemoteCommandEvent*) event;
```

## Discussion

Call the addTarget(_:action:) method multiple times to specify multiple target-action pairs. If a specific target-action pair has already been added, the request is ignored. You can add multiple actions for a single target by calling this method multiple times using the same target, but different actions.

The command object does not keep a strong reference to the target; you should remove the target before the target is deallocated.

## See Also

### Handling events

func addTarget(handler: (MPRemoteCommandEvent) -> MPRemoteCommandHandlerStatus) -> Any

Adds a block to be called when an event is received.

func removeTarget(Any?)

Removes a target from the remote command object.

func removeTarget(Any, action: Selector?)

Removes a target and action from a remote command object.

enum MPRemoteCommandHandlerStatus

Constants indicating the status of a command.

