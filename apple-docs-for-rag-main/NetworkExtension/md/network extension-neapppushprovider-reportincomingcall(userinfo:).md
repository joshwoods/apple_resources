

- Network Extension
- NEAppPushProvider
-  reportIncomingCall(userInfo:) 

Instance Method

# reportIncomingCall(userInfo:)

Informs the manager about an incoming call.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func reportIncomingCall(userInfo: [AnyHashable : Any] = [:])
```

## Parameters 

`userInfo`  

A dictionary of custom information associated with the incoming call. The dictionary’s values must only use data types supported by PropertyListSerialization; you can’t use custom types for the values.

## Discussion

Call this method when your provider determines it’s receiving an incoming call on the connection. The manager’s delegate receives this dictionary as-is.

## See Also

### Receiving local events

func reportPushToTalkMessage(userInfo: [AnyHashable : Any])

Informs the manager about a push-to-talk message on the connection.

