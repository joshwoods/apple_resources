

- Bundle Resources
- Entitlements
-  APS Environment (macOS) Entitlement 

Property List Key

# APS Environment (macOS) Entitlement

The environment for push notifications in macOS apps.

macOS 10.14+

## Details 

Key  
com.apple.developer.aps-environment

Type  

string

## Possible Values 

`development`  

The APNs development environment.

`production`  

The APNs production environment.

## Discussion

This key specifies whether to use the development or production Apple Push Notification service (APNs) environment when registering for push notifications with registerForRemoteNotifications().

Xcode sets the value of the entitlement based on your app’s current provisioning profile. For example, if you’re using a development provisioning profile, Xcode sets the value to `development`.

To add this entitlement to your app, enable the Push Notifications capability in Xcode.

## See Also

### Related Documentation

Registering your app with APNs

Communicate with Apple Push Notification service (APNs) and receive a unique device token that identifies your app.

### Notifications

APS Environment Entitlement

The environment for push notifications.

**Key:** aps-environment

com.apple.developer.usernotifications.filtering

Enable receiving notifications without displaying the notification to the user.

