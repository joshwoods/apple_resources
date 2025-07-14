

- Push to Talk
- PTChannelManagerDelegate
-  channelManager(\_:failedToLeaveChannel:error:) 

Instance Method

# channelManager(\_:failedToLeaveChannel:error:)

Tells the observer that the app failed to leave a Push to Talk channel.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
optional func channelManager(
    _ channelManager: PTChannelManager,
    failedToLeaveChannel channelUUID: UUID,
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

## See Also

### Joining and leaving a channel

func channelManager(PTChannelManager, didJoinChannel: UUID, reason: PTChannelJoinReason)

Tells the observer that the app successfully joined a Push to Talk channel.

**Required**

func channelManager(PTChannelManager, didLeaveChannel: UUID, reason: PTChannelLeaveReason)

Tells the observer that the app left a Push to Talk channel.

**Required**

func channelManager(PTChannelManager, failedToJoinChannel: UUID, error: any Error)

Tells the observer that the app failed to join a Push to Talk channel.

