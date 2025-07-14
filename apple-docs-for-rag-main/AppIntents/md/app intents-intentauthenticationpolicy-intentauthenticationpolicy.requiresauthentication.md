

- App Intents
- IntentAuthenticationPolicy
-  IntentAuthenticationPolicy.requiresAuthentication 

Case

# IntentAuthenticationPolicy.requiresAuthentication

A policy that requires the user to authenticate.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
case requiresAuthentication
```

## Discussion

If the device is in a locked state and the request doesn’t originate on an authenticated remote device; for example a connected Apple Watch; the system prompts a person to unlock the device before it runs the app intent.

## See Also

### Authentication policies

case alwaysAllowed

A policy that allows the app intent to always run, even on a locked device.

case requiresLocalDeviceAuthentication

A policy that requires the user to authenticate on the local device.

