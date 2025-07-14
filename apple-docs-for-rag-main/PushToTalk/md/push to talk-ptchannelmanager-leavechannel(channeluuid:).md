

- Push to Talk
- PTChannelManager
-  leaveChannel(channelUUID:) 

Instance Method

# leaveChannel(channelUUID:)

Leaves a channel with the identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func leaveChannel(channelUUID: UUID)
```

## Parameters 

`channelUUID`  

The channel identifier.

## Discussion

If successful, you receive a callback from channelManager(_:didLeaveChannel:reason:) with `PTChannelLeaveReason.programmaticRequest`; otherwise, you receive a failure reason through channelManager(_:failedToLeaveChannel:error:).

## See Also

### Joining and leaving a channel

func requestJoinChannel(channelUUID: UUID, descriptor: PTChannelDescriptor)

Joins a channel with the identifier and descriptor you specify.

