

- App Intents
- IntentAuthenticationPolicy
-  IntentAuthenticationPolicy.requiresLocalDeviceAuthentication 

Case

# IntentAuthenticationPolicy.requiresLocalDeviceAuthentication

A policy that requires the user to authenticate on the local device.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
case requiresLocalDeviceAuthentication
```

## Discussion

Use this policy if your app intent relies on data or services that are only available when the device is unlocked. The system always prompts a person to unlock if their device is locked, even when the request originates on an authenticated remote device; for example, their connected Apple Watch.

## See Also

### Authentication policies

case alwaysAllowed

A policy that allows the app intent to always run, even on a locked device.

case requiresAuthentication

A policy that requires the user to authenticate.

