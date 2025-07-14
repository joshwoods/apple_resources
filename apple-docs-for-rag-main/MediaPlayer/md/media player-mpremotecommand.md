

- Media Player
-  MPRemoteCommand 

Class

# MPRemoteCommand

An object that responds to remote command events.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+watchOS 5.0+

``` source
class MPRemoteCommand
```

## Overview

The Media Player framework defines a standard set of remote command objects for handling media-related events. When an accessory or iOS user interface generates a remote control event, the system notifies the corresponding command object on the shared MPRemoteCommandCenter instance. That command object executes any attached handlers.

To respond to a particular event, register a handler with the appropriate MPRemoteCommand object.

Listing 1. Registering a remote control event handler

- Swift
- Objective-C

```
// Get the shared command center.
let commandCenter = MPRemoteCommandCenter.shared()

// Add a handler for the play command.
commandCenter.playCommand.addTarget { [unowned self] event in
    if self.player.rate == 0.0 {
        self.player.play()
        return .success
    }
    return .commandFailed
}
```

```
// Get the shared command center.
MPRemoteCommandCenter *commandCenter = [MPRemoteCommandCenter sharedCommandCenter];

// Add a handler for the play command.
[commandCenter.playCommand addTargetWithHandler:^MPRemoteCommandHandlerStatus(MPRemoteCommandEvent * _Nonnull event) {
    if (self.player.rate == 0.0) {
        [self.player play];
        return MPRemoteCommandHandlerStatusSuccess;
    }
    return MPRemoteCommandHandlerStatusCommandFailed;
}];
```

If you explicitly don’t want to enable a given command, fetch the command object and set its enabled property to false. Disabling a remote command lets the system know that it shouldn’t display any related UI for that command when your app is the Now Playing app.

The framework defines many subclasses to handle specific kinds of commands. Sometimes, these subclasses let you specify other information related to the command. For example, feedback commands let you specify a localized string that describes the meaning of the feedback. When supporting a particular command, be sure to look up the specific class used to handle those events.

## Topics

### Handling events

func addTarget(handler: (MPRemoteCommandEvent) -> MPRemoteCommandHandlerStatus) -> Any

Adds a block to be called when an event is received.

func addTarget(Any, action: Selector)

Adds a target object to be called when an event is received.

func removeTarget(Any?)

Removes a target from the remote command object.

func removeTarget(Any, action: Selector?)

Removes a target and action from a remote command object.

enum MPRemoteCommandHandlerStatus

Constants indicating the status of a command.

### Enabling a command object

var isEnabled: Bool

A Boolean value that indicates whether a user can interact with the displayed element.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MPChangePlaybackPositionCommand
- MPChangePlaybackRateCommand
- MPChangeRepeatModeCommand
- MPChangeShuffleModeCommand
- MPFeedbackCommand
- MPRatingCommand
- MPSkipIntervalCommand

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Setting up the remote event handler

Becoming a now playable app

Ensure your app is eligible to become the Now Playing app by adopting best practices for providing Now Playing info and registering for remote command center actions.

class MPRemoteCommandCenter

An object that responds to remote control events sent by external accessories and system controls.

class MPRemoteCommandEvent

A description of a command sent by an external media player.

