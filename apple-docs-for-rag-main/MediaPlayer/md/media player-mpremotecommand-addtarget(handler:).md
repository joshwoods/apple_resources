

- Media Player
- MPRemoteCommand
-  addTarget(handler:) 

Instance Method

# addTarget(handler:)

Adds a block to be called when an event is received.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
func addTarget(handler: @escaping (MPRemoteCommandEvent) -> MPRemoteCommandHandlerStatus) -> Any
```

## Parameters 

`handler`  

A block object to handle the MPRemoteCommandEvent.

## Return Value

An opaque object associated with the designated handler.

## Discussion

Call the addTarget(handler:) method to add a block to be called. Remove the handler by calling the removeTarget(_:) method, passing in the object returned by this method.

## See Also

### Handling events

func addTarget(Any, action: Selector)

Adds a target object to be called when an event is received.

func removeTarget(Any?)

Removes a target from the remote command object.

func removeTarget(Any, action: Selector?)

Removes a target and action from a remote command object.

enum MPRemoteCommandHandlerStatus

Constants indicating the status of a command.

