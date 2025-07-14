

- Push to Talk
- PTChannelManager
-  setActiveRemoteParticipant(\_:channelUUID:completionHandler:) 

Instance Method

# setActiveRemoteParticipant(\_:channelUUID:completionHandler:)

Sets the active remote participant with the channel identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func setActiveRemoteParticipant(
    _ participant: PTParticipant?,
    channelUUID: UUID,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func setActiveRemoteParticipant(
    _ participant: PTParticipant?,
    channelUUID: UUID
) async throws
```

## Parameters 

`participant`  

The remote participant to become active.

`channelUUID`  

The channel identifier the participant becomes active in.

`completionHandler`  

The completion handler that contains an optional error.

`error`  
An error, if any, that indicates the reason why the system couldn’t set the active participant.

## Mentioned in 

Creating a Push to Talk app

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func setActiveRemoteParticipant(_ participant: PTParticipant?, channelUUID: UUID) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

When you receive incoming audio from a remote participant, set the participant value, which updates the system user interface and blocks transmission by the local user. When the user stops speaking, set the active participant to `nil`.

