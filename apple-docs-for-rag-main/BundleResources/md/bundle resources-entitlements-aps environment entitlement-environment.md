

- Bundle Resources
- Entitlements
-  APS Environment Entitlement 

Property List Key

# APS Environment Entitlement

The environment for push notifications.

iOS 10.0+iPadOS 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

## Details 

Key  
aps-environment

Type  

string

## Possible Values 

`development`  

The APNs development environment.

`production`  

The APNs production environment.

## Discussion

This key specifies whether to use the development or production Apple Push Notification service (APNs) environment when registering for push notifications.

Xcode sets the value of the entitlement based on your app’s current provisioning profile. For example, if you’re using a development provisioning profile, Xcode sets the value to `development`. Production provisioning profile and Prerelease Versions and Beta Testers use `production`. These default settings can be modified. The `development` environment is also referred to as the `sandbox` environment.

Use this entitlement for both the UserNotifications and PushKit frameworks.

To add this entitlement to your app, enable the Push Notifications capability in Xcode.

## See Also

### Related Documentation

Registering your app with APNs

Communicate with Apple Push Notification service (APNs) and receive a unique device token that identifies your app.

PushKit

Respond to push notifications related to your app’s complications, file providers, and VoIP services.

### Notifications

APS Environment (macOS) Entitlement

The environment for push notifications in macOS apps.

**Key:** com.apple.developer.aps-environment

com.apple.developer.usernotifications.filtering

Enable receiving notifications without displaying the notification to the user.

