

- Push to Talk
- PTChannelManager
-  setTransmissionMode(\_:channelUUID:completionHandler:) 

Instance Method

# setTransmissionMode(\_:channelUUID:completionHandler:)

Sets the audio transmission mode for the channel you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func setTransmissionMode(
    _ transmissionMode: PTTransmissionMode,
    channelUUID: UUID,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func setTransmissionMode(
    _ transmissionMode: PTTransmissionMode,
    channelUUID: UUID
) async throws
```

## Parameters 

`transmissionMode`  

The transmission mode.

`channelUUID`  

The channel identifier the participant becomes active in.

`completionHandler`  

The completion handler that contains an optional error.

`error`  
An error, if any, that indicates the reason why the system couldn’t set the transmission mode.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func setTransmissionMode(_ transmissionMode: PTTransmissionMode, channelUUID: UUID) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

By default, a channel’s transmission mode is PTTransmissionMode.halfDuplex — indicating that only one participant can send or receive audio at a time. Use PTTransmissionMode.fullDuplex to allow a person to transmit and receive audio simultaneously.

Set the transmission mode to PTTransmissionMode.listenOnly to prevent a participant from transmitting any audio.

