

- Push to Talk
- PTChannelManagerDelegate
-  incomingPushResult(channelManager:channelUUID:pushPayload:) 

Instance Method

# incomingPushResult(channelManager:channelUUID:pushPayload:)

Tells the observer that the app has a push available to handle.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func incomingPushResult(
    channelManager: PTChannelManager,
    channelUUID: UUID,
    pushPayload: [String : Any]
) -> PTPushResult
```

**Required**

## Parameters 

`channelManager`  

The channel manager.

`channelUUID`  

The channel identifier.

`pushPayload`  

The push payload metadata.

## Mentioned in 

Creating a Push to Talk app

## Discussion

The system calls this method for each incoming push. Return a PTPushResult as soon as possible and don’t block the thread. Perform network tasks — like downloading a speaker’s image or setting up a streaming network connection to a server — on a separate thread.

If the PTT channel transmission mode is PTTransmissionMode.halfDuplex, and the local participant is transmitting when the app receives a PTT notification, returning an active participant results in an error. End the local participant’s transmission by calling stopTransmitting(channelUUID:) before returning an active remote participant.

