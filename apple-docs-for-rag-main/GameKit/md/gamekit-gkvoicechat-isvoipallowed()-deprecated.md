

- GameKit
- GKVoiceChat
-  isVoIPAllowed() Deprecated

Type Method

# isVoIPAllowed()

Returns whether voice chat is available on the device.

iOS 4.1–18.0DeprecatediPadOS 4.1–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.8–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
class func isVoIPAllowed() -> Bool
```

Deprecated

No longer supported

## Return Value

true if voice chat is available to the game.

## Discussion

Some countries or phone carriers may restrict the availability of Voice-over-IP (VoIP) services. Before creating a `GKVoiceChat` object, your game should first check to see whether the device supports VoIP.

