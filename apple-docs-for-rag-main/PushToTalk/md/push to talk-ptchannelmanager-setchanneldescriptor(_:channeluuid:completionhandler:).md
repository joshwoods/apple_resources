

- Push to Talk
- PTChannelManager
-  setChannelDescriptor(\_:channelUUID:completionHandler:) 

Instance Method

# setChannelDescriptor(\_:channelUUID:completionHandler:)

Sets the channel description.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func setChannelDescriptor(
    _ channelDescriptor: PTChannelDescriptor,
    channelUUID: UUID,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func setChannelDescriptor(
    _ channelDescriptor: PTChannelDescriptor,
    channelUUID: UUID
) async throws
```

## Parameters 

`channelDescriptor`  

The channel description.

`channelUUID`  

The channel identifier.

`completionHandler`  

The completion handler.

`error`  
An error, if any, that indicates the reason why the system couldn’t set the channel descriptor.

## Mentioned in 

Creating a Push to Talk app

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func setChannelDescriptor(_ channelDescriptor: PTChannelDescriptor, channelUUID: UUID) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

