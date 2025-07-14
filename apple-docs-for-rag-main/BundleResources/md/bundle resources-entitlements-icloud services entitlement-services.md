

- Bundle Resources
- Entitlements
-  iCloud Services Entitlement 

Property List Key

# iCloud Services Entitlement

The iCloud services used by the app.

iOS 3.0+iPadOS 3.0+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

## Details 

Key  
com.apple.developer.icloud-services

Type  

array of strings

## Possible Values 

`CloudDocuments`  

`CloudKit`  

`CloudKit-Anonymous`  

## Discussion

To add this entitlement to your app, enable the iCloud capability and the iCloud Documents or CloudKit service in Xcode.

The value `CloudKit-Anonymous` is only available to App Clips, but App Clips can’t use the values `CloudDocuments` or `CloudKit`. For more information on using CloudKit in your App Clip, see Sharing data between your App Clip and your full app.

## See Also

### iCloud

com.apple.developer.icloud-container-development-container-identifiers

The container identifiers for the iCloud development environment.

com.apple.developer.icloud-container-environment

The development or production environment to use for the iCloud containers.

iCloud Container Identifiers Entitlement

The container identifiers for the iCloud production environment.

**Key:** com.apple.developer.icloud-container-identifiers

iCloud Key-Value Store Entitlement

The container identifier to use for iCloud key-value storage.

**Key:** com.apple.developer.ubiquity-kvstore-identifier

