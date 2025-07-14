

- Bundle Resources
- Entitlements
-  com.apple.developer.associated-appclip-app-identifiers 

Property List Key

# com.apple.developer.associated-appclip-app-identifiers

A list of App Clip identifiers for an app with exactly one entry.

iOS 15.4+iPadOS 15.4+

## Details 

Type  

array of strings

## Discussion

The `com.apple.developer.associated-appclip-app-identifiers` entitlement provides an app with the bundle ID of its associated App Clip. Together with the Parent Application Identifiers Entitlement, the Associated App Clip Identifiers entitlement establishes an association between your App Clip and your app that the system uses to enable data sharing between them. For additional information on sharing data between your App Clip and your full app, see Sharing data between your App Clip and your full app.

Note

Xcode adds this entitlement when you archive an app that includes an App Clip.

## See Also

### App Clips

Parent Application Identifiers Entitlement

A list of parent application identifiers for an App Clip with exactly one entry.

**Key:** com.apple.developer.parent-application-identifiers

com.apple.developer.on-demand-install-capable

A Boolean value that indicates whether a bundle represents an App Clip.

