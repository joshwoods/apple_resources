

- Push to Talk
- PTChannelManager
-  setAccessoryButtonEventsEnabled(\_:channelUUID:completionHandler:) 

Instance Method

# setAccessoryButtonEventsEnabled(\_:channelUUID:completionHandler:)

Maps supported accessory button events to actions that begin and end transmission.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
func setAccessoryButtonEventsEnabled(
    _ enabled: Bool,
    channelUUID: UUID,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func setAccessoryButtonEventsEnabled(
    _ enabled: Bool,
    channelUUID: UUID
) async throws
```

## Parameters 

`enabled`  

A flag that accessory button events map to begin and end transmission actions. If your app doesn’t map these button events to transmission actions, you can disable them by setting the value to false.

`channelUUID`  

The unique channel identifier of the active participant.

`completionHandler`  

An error that indicates the reason why the system couldn’t set the supported accessory button events.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func setAccessoryButtonEventsEnabled(_ enabled: Bool, channelUUID: UUID) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Starting and stopping transmission

func requestBeginTransmitting(channelUUID: UUID)

Begins an audio transmission with the channel identifer you specify.

func stopTransmitting(channelUUID: UUID)

Stops an audio transmission with the channel identifer you specify.

