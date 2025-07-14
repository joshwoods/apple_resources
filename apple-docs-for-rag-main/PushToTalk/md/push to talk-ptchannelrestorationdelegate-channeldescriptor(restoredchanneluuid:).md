

- Push to Talk
- PTChannelRestorationDelegate
-  channelDescriptor(restoredChannelUUID:) 

Instance Method

# channelDescriptor(restoredChannelUUID:)

Tells your observer the system restored the channel.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func channelDescriptor(restoredChannelUUID channelUUID: UUID) -> PTChannelDescriptor
```

**Required**

## Parameters 

`channelUUID`  

The channel identifier.

## Return Value

An object that describes a channel you associate with the unique identifier.

## Mentioned in 

Creating a Push to Talk app

## Discussion

If the system tracks a channel, but there’s no pending push, the system calls this method when it’s unable to use cached data. If your app launches because of user interaction with the system user interface, the system calls this method as long as there’s no pending push.

