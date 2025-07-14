

- PushKit
- PKPushRegistryDelegate
-  pushRegistry(\_:didReceiveIncomingPushWith:for:completion:) 

Instance Method

# pushRegistry(\_:didReceiveIncomingPushWith:for:completion:)

Tells the delegate that a remote push notification arrived.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
optional func pushRegistry(
    _ registry: PKPushRegistry,
    didReceiveIncomingPushWith payload: PKPushPayload,
    for type: PKPushType,
    completion: @escaping () -> Void
)
```

``` source
optional func pushRegistry(
    _ registry: PKPushRegistry,
    didReceiveIncomingPushWith payload: PKPushPayload,
    for type: PKPushType
) async
```

## Parameters 

`registry`  

The PKPushRegistry instance responsible for the delegate callback.

`payload`  

The push payload sent by a developer via APNs server API.

`type`  

This is a PKPushType constant, which is present in `[registry desiredPushTypes]`.

`completion`  

The notification’s completion handler. Execute this block when you finish processing the notification.

## Mentioned in 

Responding to VoIP Notifications from PushKit

## Discussion

Concurrency note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func pushRegistry(_ registry: PKPushRegistry, didReceiveIncomingPushWith payload: PKPushPayload, for type: PKPushType) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The system calls this method when it receives a push notification for the specified push type. Use this method to extract data from the notification’s payload and to perform the relevant task for that data. For example, use this method to update the complication data of your watchOS app. When you finish the task, execute the provided `completion` handler block to let PushKit know you are finished.

When linking against the iOS 13 SDK or later, your implementation of this method must report notifications of type voIP to the CallKit framework by calling the reportNewIncomingCall(with:update:completion:) method of your app’s `CXProvider` object. When you call that method, the system displays the standard incoming call interface to the user unless an error occurs. For example, the system reports an error if the user enabled Do Not Disturb. You may establish a connection to your VoIP server in tandem with notify CallKit.

Important

On iOS 13.0 and later, if you fail to report a call to CallKit, the system will terminate your app. Repeatedly failing to report calls may cause the system to stop delivering any more VoIP push notifications to your app. If you want to initiate a VoIP call without using CallKit, register for push notifications using the User Notifications framework instead of PushKit. For more information, see User Notifications.

