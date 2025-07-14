

- Bundle Resources
- Entitlements
-  com.apple.developer.coremotion.head-pose 

Property List Key

# com.apple.developer.coremotion.head-pose

An entitlement that enables someone’s head movement to determine the orientation of spatialized sound output.

iOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+

## Details 

Type  

boolean

## Discussion

This entitlement changes the orientation of spatial audio output to match the person’s head pose via compatible AirPods for the following APIs:

- AVAudioEnvironmentNode, when you set the isListenerHeadTrackingEnabled property to `true`

- Audio Toolbox (see AUSpatialMixer Parameters), when you set the kAudioUnitProperty_SpatialMixerEnableHeadTracking property to `true`

- PHASEListener, when you set the new automaticHeadTrackingFlags property to orientation

Add this entitlement to your app by enabling the Head Pose capability in Xcode.

## See Also

### Media

Media Device Discovery Extension

An entitlement for an app extension that adds a specific third-party media receiver to a system device-picker UI.

**Key:** com.apple.developer.media-device-discovery-extension

com.apple.developer.spatial-audio.profile-access

An entitlement that enables your app to use the personalized spatial audio profile.

com.apple.developer.avfoundation.multitasking-camera-access

A Boolean value that indicates whether an app may continue using the camera at the same time as another foreground app.

Deprecated

