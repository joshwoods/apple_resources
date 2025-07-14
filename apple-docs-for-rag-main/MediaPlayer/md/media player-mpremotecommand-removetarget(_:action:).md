

- Media Player
- MPRemoteCommand
-  removeTarget(\_:action:) 

Instance Method

# removeTarget(\_:action:)

Removes a target and action from a remote command object.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
func removeTarget(
    _ target: Any,
    action: Selector?
)
```

## Parameters 

`target`  

The object that currently is a recipient of action messages sent by this object. Specify `nil` to remove all targets.

`action`  

A selector identifying a method on the target. Specify `NULL` to remove all actions.

## Discussion

Call the removeTarget(_:action:) method to remove the specified target-action pair. Passing `nil` for `target` matches all targets and passing `NULL` for `action` matches all actions.

## See Also

### Handling events

func addTarget(handler: (MPRemoteCommandEvent) -> MPRemoteCommandHandlerStatus) -> Any

Adds a block to be called when an event is received.

func addTarget(Any, action: Selector)

Adds a target object to be called when an event is received.

func removeTarget(Any?)

Removes a target from the remote command object.

enum MPRemoteCommandHandlerStatus

Constants indicating the status of a command.

