

- Bundle Resources
- Entitlements
-  Inter-App Audio Entitlement Deprecated

Property List Key

# Inter-App Audio Entitlement

A Boolean value that indicates whether the app may exchange audio with other Inter-App Audio-enabled apps.

iOS 2.2–13.0DeprecatediPadOS 2.2–13.0Deprecated

Deprecated

Inter-App Audio is deprecated in iOS 13 and is unavailable when running iPad apps in macOS.

## Details 

Key  
inter-app-audio

Type  

boolean

## Discussion

Enabling Inter-App Audio allows your app to send and receive audio from other Inter-App Audio enabled apps and provides access to Audio Unit extensions.

To add this entitlement to your app, enable the Inter-App Audio capability in Xcode.

## See Also

### Deprecated entitlements

Maps Entitlement

A Boolean value that indicates whether the app may provide directions beyond what Maps supports, such as subway routes, hiking trails, and bike paths.

**Key:** com.apple.developer.maps

Deprecated

All files entitlement

A Boolean value that indicates whether the app may have access to all files.

**Key:** com.apple.security.files.all

Deprecated

