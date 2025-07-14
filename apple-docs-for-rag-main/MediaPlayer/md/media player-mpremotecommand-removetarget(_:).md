

- Media Player
- MPRemoteCommand
-  removeTarget(\_:) 

Instance Method

# removeTarget(\_:)

Removes a target from the remote command object.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
func removeTarget(_ target: Any?)
```

## Parameters 

`target`  

The object that currently is a recipient of action messages sent by this object. Specify `nil` to remove all targets.

## Discussion

Call the removeTarget(_:) method to remove the specified target and all actions associated with the target.

## See Also

### Handling events

func addTarget(handler: (MPRemoteCommandEvent) -> MPRemoteCommandHandlerStatus) -> Any

Adds a block to be called when an event is received.

func addTarget(Any, action: Selector)

Adds a target object to be called when an event is received.

func removeTarget(Any, action: Selector?)

Removes a target and action from a remote command object.

enum MPRemoteCommandHandlerStatus

Constants indicating the status of a command.

