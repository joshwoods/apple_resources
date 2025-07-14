

- GameKit
- GKVoiceChatService
-  isVoIPAllowed() Deprecated

Type Method

# isVoIPAllowed()

Returns whether voice chat is allowed to be used on the device.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
class func isVoIPAllowed() -> Bool
```

Deprecated

Use SharePlay instead

## Return Value

true if voice chat is available to the application.

## Discussion

Some countries or phone carriers may restrict the availability of voice over IP services. Before retrieving the shared voice chat service object, your application should check to see whether voice chat is available.

