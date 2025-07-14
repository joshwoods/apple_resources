

- Push to Talk
- PTChannelManager
-  requestBeginTransmitting(channelUUID:) 

Instance Method

# requestBeginTransmitting(channelUUID:)

Begins an audio transmission with the channel identifer you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func requestBeginTransmitting(channelUUID: UUID)
```

## Parameters 

`channelUUID`  

The channel identifier.

## Mentioned in 

Creating a Push to Talk app

## Discussion

Your app can only begin a transmission when in the foreground, or following a Core Bluetooth event, such as when a wireless accessory button triggers a Core Bluetooth characteristic change. The user may also begin a transmission by using the Push to Talk system user interface.

If successful, you receive a callback from channelManager(_:channelUUID:didBeginTransmittingFrom:) with `PTChannelTransmitRequestSource.programmaticRequest`; otherwise, you receive a failure reason through channelManager(_:failedToBeginTransmittingInChannel:error:).

## See Also

### Starting and stopping transmission

func stopTransmitting(channelUUID: UUID)

Stops an audio transmission with the channel identifer you specify.

func setAccessoryButtonEventsEnabled(Bool, channelUUID: UUID, completionHandler: (((any Error)?) -> Void)?)

Maps supported accessory button events to actions that begin and end transmission.

