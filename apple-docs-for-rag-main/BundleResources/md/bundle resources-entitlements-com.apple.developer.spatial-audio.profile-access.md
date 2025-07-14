

- Bundle Resources
- Entitlements
-  com.apple.developer.spatial-audio.profile-access 

Property List Key

# com.apple.developer.spatial-audio.profile-access

An entitlement that enables your app to use the personalized spatial audio profile.

iOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

## Details 

Type  

boolean

## Discussion

This entitlement applies the personalized spatial audio profile someone makes in Settings to your app’s audio output for the following APIs:

- AVAudioEngine

- AUSpatialMixer in Audio Toolbox (see AUSpatialMixer Parameters)

- PHASE

Add this entitlement to your app by enabling the Spatial Audio Profile capability in Xcode.

Note

In iOS 18 and tvOS 18 and later, the system automatically adds spatial audio to the output for games. To opt out of automatic spatial audio and support just your preferred spatial audio setup, add the AVGameBypassSystemSpatialAudio key to your app’s `Info.plist`.

## See Also

### Media

Media Device Discovery Extension

An entitlement for an app extension that adds a specific third-party media receiver to a system device-picker UI.

**Key:** com.apple.developer.media-device-discovery-extension

com.apple.developer.coremotion.head-pose

An entitlement that enables someone’s head movement to determine the orientation of spatialized sound output.

com.apple.developer.avfoundation.multitasking-camera-access

A Boolean value that indicates whether an app may continue using the camera at the same time as another foreground app.

Deprecated

