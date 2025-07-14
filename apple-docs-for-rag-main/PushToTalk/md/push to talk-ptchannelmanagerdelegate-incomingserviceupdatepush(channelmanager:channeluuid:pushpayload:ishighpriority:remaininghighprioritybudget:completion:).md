

- Push to Talk
- PTChannelManagerDelegate
-  incomingServiceUpdatePush(channelManager:channelUUID:pushPayload:isHighPriority:remainingHighPriorityBudget:completion:) 

Instance Method

# incomingServiceUpdatePush(channelManager:channelUUID:pushPayload:isHighPriority:remainingHighPriorityBudget:completion:)

Extracts the service update data from the notification’s payload to perform the relevant task for that data.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+

``` source
optional func incomingServiceUpdatePush(
    channelManager: PTChannelManager,
    channelUUID: UUID,
    pushPayload: [String : Any],
    isHighPriority: Bool,
    remainingHighPriorityBudget: Int,
    completion: @escaping () -> Void
)
```

``` source
optional func incomingServiceUpdatePush(
    channelManager: PTChannelManager,
    channelUUID: UUID,
    pushPayload: [String : Any],
    isHighPriority: Bool,
    remainingHighPriorityBudget: Int
) async
```

## Parameters 

`channelManager`  

The channel manager.

`channelUUID`  

The channel identifier.

`pushPayload`  

The push payload metadata.

`isHighPriority`  

A flag indicating if this notification is a high priority.

`remainingHighPriorityBudget`  

Monitors the number of remaining high-priority push notifications available to your app. Use low-priority push notifications (priority \

`completion`  

Execute to inform the Push to Talk framework you’ve finished your task.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func incomingServiceUpdatePush(channelManager: PTChannelManager, channelUUID: UUID, pushPayload: [String : Any], isHighPriority: Bool, remainingHighPriorityBudget: Int) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

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

func channelManager(PTChannelManager, failedToStopTransmittingInChannel: UUID, error: any Error)

Tells the observer that transmission failed to stop.

