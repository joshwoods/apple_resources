

- PushKit
- PKPushCredentials
-  token 

Instance Property

# token

A unique device token to use when sending push notifications to the current device.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
var token: Data { get }
```

## Discussion

Forward this token to the server you use to generate push notifications. When preparing to deliver a push notification to the current device, include the token in the HTTP request you send to Apple Push Notification service (APNs).

## See Also

### Getting the Token

var type: PKPushType

The push type constant associated with the token.

