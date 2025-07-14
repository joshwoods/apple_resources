

- Network Extension
- NEAppPushProvider
-  reportPushToTalkMessage(userInfo:) 

Instance Method

# reportPushToTalkMessage(userInfo:)

Informs the manager about a push-to-talk message on the connection.

iOS 16.4+iPadOS 16.4+visionOS 1.0+

``` source
func reportPushToTalkMessage(userInfo: [AnyHashable : Any] = [:])
```

## Parameters 

`userInfo`  

A dictionary of custom information associated with the push-to -talk message, such as the active remote participant. The containing app’s PTChannelManagerDelegate receives this dictionary if the user has joined a push-to-talk channel.

## See Also

### Receiving local events

func reportIncomingCall(userInfo: [AnyHashable : Any])

Informs the manager about an incoming call.

