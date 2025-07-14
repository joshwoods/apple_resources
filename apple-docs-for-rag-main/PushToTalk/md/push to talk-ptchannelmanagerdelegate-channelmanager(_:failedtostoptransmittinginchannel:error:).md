

- Push to Talk
- PTChannelManagerDelegate
-  channelManager(\_:failedToStopTransmittingInChannel:error:) 

Instance Method

# channelManager(\_:failedToStopTransmittingInChannel:error:)

Tells the observer that transmission failed to stop.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
optional func channelManager(
    _ channelManager: PTChannelManager,
    failedToStopTransmittingInChannel channelUUID: UUID,
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

### Beginning or ending transmission

func channelManager(PTChannelManager, channelUUID: UUID, didBeginTransmittingFrom: PTChannelTransmitRequestSource)

Tells the observer that transmission began.

**Required**

func channelManager(PTChannelManager, channelUUID: UUID, didEndTransmittingFrom: PTChannelTransmitRequestSource)

Tells the observer that transmission ended.

**Required**

func channelManager(PTChannelManager, failedToBeginTransmittingInChannel: UUID, error: any Error)

Tells the observer that transmission failed to begin.

func incomingServiceUpdatePush(channelManager: PTChannelManager, channelUUID: UUID, pushPayload: [String : Any], isHighPriority: Bool, remainingHighPriorityBudget: Int, completion: () -> Void)

Extracts the service update data from the notification’s payload to perform the relevant task for that data.

