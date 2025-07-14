

- Push to Talk
-  PTChannelManager 

Class

# PTChannelManager

An object that represents a push-to-talk channel manager.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
class PTChannelManager
```

## Mentioned in 

Creating a Push to Talk app

## Overview

You must create a channel manager upon launching your app, otherwise the system tears down channels and their ability to receive push notifications. By providing a PTChannelRestorationDelegate, an app can rejoin or leave a previously active channel the system knows about. Once the channel resoration process completes, the system provides a PTChannelManager instance.

```
// Create a channel manager instance.    
channelManager = try await PTChannelManager.channelManager(delegate: self,
                                                           restorationDelegate: self)
```

Multiple calls to channelManager(delegate:restorationDelegate:completionHandler:) result in the system returning the same shared instance, so store the channel manager in an instance variable.

## Topics

### Creating a channel manager

class func channelManager(delegate: any PTChannelManagerDelegate, restorationDelegate: any PTChannelRestorationDelegate, completionHandler: (PTChannelManager?, (any Error)?) -> Void)

Creates a channel manager with the configuration you specify.

### Inspecting the channel manager

var activeChannelUUID: UUID?

The unique identifier of the active channel for the app.

### Joining and leaving a channel

func requestJoinChannel(channelUUID: UUID, descriptor: PTChannelDescriptor)

Joins a channel with the identifier and descriptor you specify.

func leaveChannel(channelUUID: UUID)

Leaves a channel with the identifier.

### Setting the transmission mode

func setTransmissionMode(PTTransmissionMode, channelUUID: UUID, completionHandler: (((any Error)?) -> Void)?)

Sets the audio transmission mode for the channel you specify.

### Starting and stopping transmission

func requestBeginTransmitting(channelUUID: UUID)

Begins an audio transmission with the channel identifer you specify.

func stopTransmitting(channelUUID: UUID)

Stops an audio transmission with the channel identifer you specify.

func setAccessoryButtonEventsEnabled(Bool, channelUUID: UUID, completionHandler: (((any Error)?) -> Void)?)

Maps supported accessory button events to actions that begin and end transmission.

### Setting participants

func setActiveRemoteParticipant(PTParticipant?, channelUUID: UUID, completionHandler: (((any Error)?) -> Void)?)

Sets the active remote participant with the channel identifier.

### Setting the channel descriptor

func setChannelDescriptor(PTChannelDescriptor, channelUUID: UUID, completionHandler: (((any Error)?) -> Void)?)

Sets the channel description.

### Setting the service status

func setServiceStatus(PTServiceStatus, channelUUID: UUID, completionHandler: (((any Error)?) -> Void)?)

Sets the service connection status.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Essentials

Creating a Push to Talk app

Build a walkie-talkie style app with system user interface controls.

