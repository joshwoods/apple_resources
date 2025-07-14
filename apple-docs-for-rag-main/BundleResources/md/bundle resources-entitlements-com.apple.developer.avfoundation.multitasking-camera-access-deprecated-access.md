

- Bundle Resources
- Entitlements
-  com.apple.developer.avfoundation.multitasking-camera-access Deprecated

Property List Key

# com.apple.developer.avfoundation.multitasking-camera-access

A Boolean value that indicates whether an app may continue using the camera at the same time as another foreground app.

iOS 13.5–18.0DeprecatediPadOS 13.5–18.0Deprecated

Deprecated

In iOS 18, the use of this entitlement is no longer required. Use isMultitaskingCameraAccessSupported instead.

## Details 

Type  

boolean

## Discussion

When your app enters a multitasking mode, this entitlement allows it to continue using the camera. Multitasking modes include Slide Over, Split View, and Picture in Picture (PiP). For information about Picture in Picture, see Adopting Picture in Picture for video calls.

Important

Your app needs to run on iOS 13.5 or later to use this entitlement. Usage of this entitlement is restricted to apps that use `voip` as one of their UIBackgroundModes.

## See Also

### Media

Media Device Discovery Extension

An entitlement for an app extension that adds a specific third-party media receiver to a system device-picker UI.

**Key:** com.apple.developer.media-device-discovery-extension

com.apple.developer.coremotion.head-pose

An entitlement that enables someone’s head movement to determine the orientation of spatialized sound output.

com.apple.developer.spatial-audio.profile-access

An entitlement that enables your app to use the personalized spatial audio profile.

