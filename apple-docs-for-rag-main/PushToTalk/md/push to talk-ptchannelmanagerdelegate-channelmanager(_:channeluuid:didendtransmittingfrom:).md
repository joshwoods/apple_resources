

- Push to Talk
- PTChannelManagerDelegate
-  channelManager(\_:channelUUID:didEndTransmittingFrom:) 

Instance Method

# channelManager(\_:channelUUID:didEndTransmittingFrom:)

Tells the observer that transmission ended.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func channelManager(
    _ channelManager: PTChannelManager,
    channelUUID: UUID,
    didEndTransmittingFrom source: PTChannelTransmitRequestSource
)
```

**Required**

## Parameters 

`channelManager`  

The channel manager.

`channelUUID`  

The channel identifier.

`source`  

The transmission request source.

## Mentioned in 

Creating a Push to Talk app

## Discussion

The system calls this method when the user stops pressing the talk button in the user interface, a programmatic transmit ends, or transmission ends from a hands-free accessory button release.

## See Also

### Beginning or ending transmission

func channelManager(PTChannelManager, channelUUID: UUID, didBeginTransmittingFrom: PTChannelTransmitRequestSource)

Tells the observer that transmission began.

**Required**

func channelManager(PTChannelManager, failedToBeginTransmittingInChannel: UUID, error: any Error)

Tells the observer that transmission failed to begin.

func channelManager(PTChannelManager, failedToStopTransmittingInChannel: UUID, error: any Error)

Tells the observer that transmission failed to stop.

func incomingServiceUpdatePush(channelManager: PTChannelManager, channelUUID: UUID, pushPayload: [String : Any], isHighPriority: Bool, remainingHighPriorityBudget: Int, completion: () -> Void)

Extracts the service update data from the notification’s payload to perform the relevant task for that data.

