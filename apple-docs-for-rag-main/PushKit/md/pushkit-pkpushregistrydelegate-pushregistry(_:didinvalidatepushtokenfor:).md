

- PushKit
- PKPushRegistryDelegate
-  pushRegistry(\_:didInvalidatePushTokenFor:) 

Instance Method

# pushRegistry(\_:didInvalidatePushTokenFor:)

Tells the delegate that the system invalidated the push token for the specified type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
optional func pushRegistry(
    _ registry: PKPushRegistry,
    didInvalidatePushTokenFor type: PKPushType
)
```

## Parameters 

`registry`  

The PKPushRegistry instance responsible for the delegate callback.

`type`  

This is a PKPushType constant, which is present in `[registry desiredPushTypes]`.

## Discussion

The system calls this method when a previously provided push token is no longer valid for use. No action is necessary on your part to reregister the push type. Instead, use this method to notify your server not to send push notifications using the matching push token.

## See Also

### Responding to Registration Events

func pushRegistry(PKPushRegistry, didUpdate: PKPushCredentials, for: PKPushType)

Tells the delegate that the system updated the credentials for the specified type of push notification.

**Required**

