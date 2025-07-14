

- Push to Talk
- PTChannelManager
-  requestJoinChannel(channelUUID:descriptor:) 

Instance Method

# requestJoinChannel(channelUUID:descriptor:)

Joins a channel with the identifier and descriptor you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func requestJoinChannel(
    channelUUID: UUID,
    descriptor: PTChannelDescriptor
)
```

## Parameters 

`channelUUID`  

The channel identifier.

`descriptor`  

The channel description.

## Mentioned in 

Creating a Push to Talk app

## Discussion

If successful, you receive a callback from channelManager(_:didJoinChannel:reason:) with `PTChannelJoinReasonProgrammaticRequest`; otherwise, you receive a failure reason through channelManager(_:failedToJoinChannel:error:).

Note

You can only join a channel in the foreground.

The framework uses shared system resources, so only one PTT channel can be active on the system at a time.

```
// Create a descriptor an app uses to join a channel.    
let channelImage = UIImage(named: "ChannelImage")    
channelDescriptor = PTChannelDescriptor(name: "The channel name",                                                                             
                                        image: channelImage)

// Join a channel with a unique identifier and descriptor.
channelManager.requestJoinChannel(channelUUID: channelUUID,
                                  descriptor: channelDescriptor)
```

The system uses the same unique identifier when interacting with the manager throughout the life of the channel, so when joining a channel, store the descriptor and UUID for later use.

## See Also

### Joining and leaving a channel

func leaveChannel(channelUUID: UUID)

Leaves a channel with the identifier.

