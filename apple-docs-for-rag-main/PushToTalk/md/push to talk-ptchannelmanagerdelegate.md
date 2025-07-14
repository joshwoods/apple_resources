

- Push to Talk
-  PTChannelManagerDelegate 

Protocol

# PTChannelManagerDelegate

A type that represents your life cycle of a channel manager.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
protocol PTChannelManagerDelegate : NSObjectProtocol
```

## Topics

### Beginning or ending transmission

func channelManager(PTChannelManager, channelUUID: UUID, didBeginTransmittingFrom: PTChannelTransmitRequestSource)

Tells the observer that transmission began.

**Required**

func channelManager(PTChannelManager, channelUUID: UUID, didEndTransmittingFrom: PTChannelTransmitRequestSource)

Tells the observer that transmission ended.

**Required**

func channelManager(PTChannelManager, failedToBeginTransmittingInChannel: UUID, error: any Error)

Tells the observer that transmission failed to begin.

func channelManager(PTChannelManager, failedToStopTransmittingInChannel: UUID, error: any Error)

Tells the observer that transmission failed to stop.

func incomingServiceUpdatePush(channelManager: PTChannelManager, channelUUID: UUID, pushPayload: [String : Any], isHighPriority: Bool, remainingHighPriorityBudget: Int, completion: () -> Void)

Extracts the service update data from the notification’s payload to perform the relevant task for that data.

### Activating and deactivating the audio session

func channelManager(PTChannelManager, didActivate: AVAudioSession)

Tells the observer the audio session activated.

**Required**

func channelManager(PTChannelManager, didDeactivate: AVAudioSession)

Tells the observer the audio session deactivated.

**Required**

### Joining and leaving a channel

func channelManager(PTChannelManager, didJoinChannel: UUID, reason: PTChannelJoinReason)

Tells the observer that the app successfully joined a Push to Talk channel.

**Required**

func channelManager(PTChannelManager, didLeaveChannel: UUID, reason: PTChannelLeaveReason)

Tells the observer that the app left a Push to Talk channel.

**Required**

func channelManager(PTChannelManager, failedToJoinChannel: UUID, error: any Error)

Tells the observer that the app failed to join a Push to Talk channel.

func channelManager(PTChannelManager, failedToLeaveChannel: UUID, error: any Error)

Tells the observer that the app failed to leave a Push to Talk channel.

### Getting a push token

func channelManager(PTChannelManager, receivedEphemeralPushToken: Data)

Tells the observer that the app received a push token after you create a channel manager.

**Required**

### Handling the push result

func incomingPushResult(channelManager: PTChannelManager, channelUUID: UUID, pushPayload: [String : Any]) -> PTPushResult

Tells the observer that the app has a push available to handle.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Channel management

enum PTTransmissionMode

Identifies the type of audio transmission modes.

enum PTServiceStatus

Identifies the type that indicates the status of the service.

enum PTChannelJoinReason

Identifies the type that indicates the join reason.

enum PTChannelLeaveReason

Identifies the type that indicates the leave reason.

enum PTChannelTransmitRequestSource

Identifies the type that indicates the transmission request source.

