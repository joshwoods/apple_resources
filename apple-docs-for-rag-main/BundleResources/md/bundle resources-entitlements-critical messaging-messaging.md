

- Bundle Resources
- Entitlements
-  Critical Messaging 

Property List Key

# Critical Messaging

A Boolean value that indicates whether an app can use the Critical Messaging API to send SMS messages.

iOS 18.2+iPadOS 18.2+watchOS 11.2+

## Details 

Key  
com.apple.developer.messages.critical-messaging

Type  

boolean

## Attributes 

Default: `NO`

## Discussion

Add the Critical Messaging entitlement to your app by following these steps:

1.  In the Xcode project navigator, select your app’s target, and then the Signing & Capabilities tab.

2.  Add a new capability by clicking the + Capability button and then type “Critical Messaging” in the search field.

3.  Double-click the Critical Messaging entry to add the entitlement to your app.

Xcode displays the Critical Messaging entitlement, along with any other entitlements, in the capabilities list under your app’s signing information. For more information on sending critical SMS messages from your app, see Sending SMS messages from an app.

## See Also

### Messages

Default Messaging App

A Boolean value that indicates whether an app can be the default messaging app on someone’s device.

**Key:** com.apple.developer.messaging-app

