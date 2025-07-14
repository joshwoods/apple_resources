

- Media Player
-  MPRemoteCommandHandlerStatus 

Enumeration

# MPRemoteCommandHandlerStatus

Constants indicating the status of a command.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOSvisionOS 1.0+watchOS 5.0+

``` source
enum MPRemoteCommandHandlerStatus
```

## Topics

### Constants

case success

The requested command executed successfully.

case noSuchContent

The requested command couldn’t execute because its required content isn’t available.

case noActionableNowPlayingItem

The requested command couldn’t execute because no Now Playing item is available.

case deviceNotFound

The requested command couldn’t execute because a required device isn’t available.

case commandFailed

The requested command failed to execute.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Handling events

func addTarget(handler: (MPRemoteCommandEvent) -> MPRemoteCommandHandlerStatus) -> Any

Adds a block to be called when an event is received.

func addTarget(Any, action: Selector)

Adds a target object to be called when an event is received.

func removeTarget(Any?)

Removes a target from the remote command object.

func removeTarget(Any, action: Selector?)

Removes a target and action from a remote command object.

