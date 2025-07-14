

- Push to Talk
- PTChannelManager
-  channelManager(delegate:restorationDelegate:completionHandler:) 

Type Method

# channelManager(delegate:restorationDelegate:completionHandler:)

Creates a channel manager with the configuration you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
class func channelManager(
    delegate: any PTChannelManagerDelegate,
    restorationDelegate: any PTChannelRestorationDelegate,
    completionHandler: @escaping (PTChannelManager?, (any Error)?) -> Void
)
```

``` source
class func channelManager(
    delegate: any PTChannelManagerDelegate,
    restorationDelegate: any PTChannelRestorationDelegate
) async throws -> PTChannelManager
```

## Parameters 

`delegate`  

An object that conforms to the channel manager protocol.

`restorationDelegate`  

An object that conforms to the channel resoration protocol.

`completionHandler`  

The completion callback handler.

`manager`  
A new channel manager instance.

`error`  
An error, if any, that indicates the reason why the system couldn’t create the channel manager.

## Mentioned in 

Creating a Push to Talk app

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func channelManager(delegate: PTChannelManagerDelegate, restorationDelegate: PTChannelRestorationDelegate) async throws -> PTChannelManager
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

You must create a channel manager as soon as possible when launching your app so the system is able to restore existing challenge and deliver push notifications to your PTChannelManagerDelegate. By providing the restoration delegate, you decide whether to rejoin or leave any previously active channel the system knows about.

