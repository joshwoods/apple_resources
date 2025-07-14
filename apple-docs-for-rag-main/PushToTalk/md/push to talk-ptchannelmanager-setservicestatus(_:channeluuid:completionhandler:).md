

- Push to Talk
- PTChannelManager
-  setServiceStatus(\_:channelUUID:completionHandler:) 

Instance Method

# setServiceStatus(\_:channelUUID:completionHandler:)

Sets the service connection status.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func setServiceStatus(
    _ status: PTServiceStatus,
    channelUUID: UUID,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func setServiceStatus(
    _ status: PTServiceStatus,
    channelUUID: UUID
) async throws
```

## Parameters 

`status`  

The service status.

`channelUUID`  

The channel identifier.

`completionHandler`  

The completion handler.

`error`  
An error, if any, that indicates the reason why the system couldn’t set the status of the service.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func setServiceStatus(_ status: PTServiceStatus, channelUUID: UUID) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The default value for the service status is PTServiceStatus.ready. Set the appropriate service status if your network connection experiences an issue. The system reflects your service status in the user interface.

