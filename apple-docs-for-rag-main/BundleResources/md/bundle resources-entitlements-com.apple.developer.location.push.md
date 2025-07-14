

- Bundle Resources
- Entitlements
-  com.apple.developer.location.push 

Property List Key

# com.apple.developer.location.push

An entitlement to enable a location-sharing app to query someone’s location in response to a push notification.

iOS 15.0+iPadOS 15.0+

## Details 

Type  

boolean

## Discussion

This entitlement enables your app to monitor for Apple Push Notification service (APNs) pushes with the `location` push type, and receive pushes in your Location Push Service Extension. For more information about the `location` push type, see Sending notification requests to APNs.

Before submitting an app with this entitlement to the App Store, you must get permission to use the entitlement. To apply for the entitlement, log in to your Apple Developer Account with an Account Holder role and fill out the request form.

After you have the permission, add the entitlement to your app by opening the project’s entitlements file in Xcode. Add the key com.apple.developer.location.push and set the corresponding value to `YES`. Without this entitlement, your code gets an error when it calls startMonitoringLocationPushes(completion:).

For more information about implementing your Location Push Service Extension, see Creating a location push service extension.

