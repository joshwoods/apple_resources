

- Push to Talk
- PTChannelManagerDelegate
-  channelManager(\_:didLeaveChannel:reason:) 

Instance Method

# channelManager(\_:didLeaveChannel:reason:)

Tells the observer that the app left a Push to Talk channel.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func channelManager(
    _ channelManager: PTChannelManager,
    didLeaveChannel channelUUID: UUID,
    reason: PTChannelLeaveReason
)
```

**Required**

## Parameters 

`channelManager`  

The channel manager.

`channelUUID`  

The channel identifier.

`reason`  

The leave reason.

## See Also

### Joining and leaving a channel

func channelManager(PTChannelManager, didJoinChannel: UUID, reason: PTChannelJoinReason)

Tells the observer that the app successfully joined a Push to Talk channel.

**Required**

func channelManager(PTChannelManager, failedToJoinChannel: UUID, error: any Error)

Tells the observer that the app failed to join a Push to Talk channel.

func channelManager(PTChannelManager, failedToLeaveChannel: UUID, error: any Error)

Tells the observer that the app failed to leave a Push to Talk channel.

