

- Push to Talk
- PTChannelManagerDelegate
-  channelManager(\_:failedToJoinChannel:error:) 

Instance Method

# channelManager(\_:failedToJoinChannel:error:)

Tells the observer that the app failed to join a Push to Talk channel.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
optional func channelManager(
    _ channelManager: PTChannelManager,
    failedToJoinChannel channelUUID: UUID,
    error: any Error
)
```

## Parameters 

`channelManager`  

The channel manager.

`channelUUID`  

The channel identifier.

`error`  

The error that indicates the failure reason.

## Mentioned in 

Creating a Push to Talk app

## See Also

### Joining and leaving a channel

func channelManager(PTChannelManager, didJoinChannel: UUID, reason: PTChannelJoinReason)

Tells the observer that the app successfully joined a Push to Talk channel.

**Required**

func channelManager(PTChannelManager, didLeaveChannel: UUID, reason: PTChannelLeaveReason)

Tells the observer that the app left a Push to Talk channel.

**Required**

func channelManager(PTChannelManager, failedToLeaveChannel: UUID, error: any Error)

Tells the observer that the app failed to leave a Push to Talk channel.

