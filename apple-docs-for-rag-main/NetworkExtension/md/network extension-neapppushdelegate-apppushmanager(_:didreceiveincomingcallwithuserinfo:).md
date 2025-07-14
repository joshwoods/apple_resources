

- Network Extension
- NEAppPushDelegate
-  appPushManager(\_:didReceiveIncomingCallWithUserInfo:) 

Instance Method

# appPushManager(\_:didReceiveIncomingCallWithUserInfo:)

A delegate method that the framework invokes when the provider reports an incoming call.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func appPushManager(
    _ manager: NEAppPushManager,
    didReceiveIncomingCallWithUserInfo userInfo: [AnyHashable : Any] = [:]
)
```

**Required**

## Parameters 

`manager`  

The local push manager that receives the call.

`userInfo`  

A dictionary of custom information that the provider supplied in its call to reportIncomingCall(userInfo:).

## Discussion

The framwork calls this method on your delegate when the provider calls the reportIncomingCall(userInfo:) method.

