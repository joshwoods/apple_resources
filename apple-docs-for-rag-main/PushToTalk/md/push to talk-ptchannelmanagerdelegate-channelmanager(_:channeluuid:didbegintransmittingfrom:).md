

- Push to Talk
- PTChannelManagerDelegate
-  channelManager(\_:channelUUID:didBeginTransmittingFrom:) 

Instance Method

# channelManager(\_:channelUUID:didBeginTransmittingFrom:)

Tells the observer that transmission began.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func channelManager(
    _ channelManager: PTChannelManager,
    channelUUID: UUID,
    didBeginTransmittingFrom source: PTChannelTransmitRequestSource
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

The system calls this method when the user begins pressing the talk button in the user interface, a programmatic transmit starts, or transmission begins from a hands-free accessory button press.

Important

Your app must wait for the system to call channelManager(_:didActivate:) before you begin recording audio from the user.

## See Also

### Beginning or ending transmission

func channelManager(PTChannelManager, channelUUID: UUID, didEndTransmittingFrom: PTChannelTransmitRequestSource)

Tells the observer that transmission ended.

**Required**

func channelManager(PTChannelManager, failedToBeginTransmittingInChannel: UUID, error: any Error)

Tells the observer that transmission failed to begin.

func channelManager(PTChannelManager, failedToStopTransmittingInChannel: UUID, error: any Error)

Tells the observer that transmission failed to stop.

func incomingServiceUpdatePush(channelManager: PTChannelManager, channelUUID: UUID, pushPayload: [String : Any], isHighPriority: Bool, remainingHighPriorityBudget: Int, completion: () -> Void)

Extracts the service update data from the notification’s payload to perform the relevant task for that data.

