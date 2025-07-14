

- Bundle Resources
- Entitlements
-  Family Controls 

Property List Key

# Family Controls

A Boolean value that indicates whether the app can request or revoke authorization to provide parental controls.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

## Details 

Key  
com.apple.developer.family-controls

Type  

boolean

## Discussion

You must add the Family Controls entitlement to your app before you call the AuthorizationCenter class’s requestAuthorization(completionHandler:) or revokeAuthorization(completionHandler:) methods.

Adding the Family Controls capability to your app automatically sets this entitlement. Before submitting your app to the App Store, you must request permission to use the entitlement. For more information, see Adding capabilities to your app.

