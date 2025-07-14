

- PushKit
- PKPushRegistryDelegate
-  pushRegistry(\_:didReceiveIncomingPushWith:for:) Deprecated

Instance Method

# pushRegistry(\_:didReceiveIncomingPushWith:for:)

Notifies the delegate that a remote push has been received.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 8.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func pushRegistry(
    _ registry: PKPushRegistry,
    didReceiveIncomingPushWith payload: PKPushPayload,
    for type: PKPushType
)
```

Deprecated

Use pushRegistry(_:didReceiveIncomingPushWith:for:completion:) instead.

## Parameters 

`registry`  

The PKPushRegistry instance responsible for the delegate callback.

`payload`  

The push payload sent by a developer via APNS server API.

`type`  

This is a PKPushType constant, which is present in `[registry desiredPushTypes]`.

## Discussion

This method is invoked when a push notification has been received for the specified push type.

