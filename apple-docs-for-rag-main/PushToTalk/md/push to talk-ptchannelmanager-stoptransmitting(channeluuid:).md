

- Push to Talk
- PTChannelManager
-  stopTransmitting(channelUUID:) 

Instance Method

# stopTransmitting(channelUUID:)

Stops an audio transmission with the channel identifer you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func stopTransmitting(channelUUID: UUID)
```

## Parameters 

`channelUUID`  

The channel identifier.

## Mentioned in 

Creating a Push to Talk app

## Discussion

If successful, you receive a callback from channelManager(_:channelUUID:didEndTransmittingFrom:) with `PTChannelTransmitRequestSource.programmaticRequest`; otherwise, you receive a failure reason through channelManager(_:failedToStopTransmittingInChannel:error:).

## See Also

### Starting and stopping transmission

func requestBeginTransmitting(channelUUID: UUID)

Begins an audio transmission with the channel identifer you specify.

func setAccessoryButtonEventsEnabled(Bool, channelUUID: UUID, completionHandler: (((any Error)?) -> Void)?)

Maps supported accessory button events to actions that begin and end transmission.

