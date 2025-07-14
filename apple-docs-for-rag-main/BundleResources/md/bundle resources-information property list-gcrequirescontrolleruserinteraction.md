

- Bundle Resources
- Information Property List
-  GCRequiresControllerUserInteraction 

Property List Key

# GCRequiresControllerUserInteraction

The platforms for which your app requires or you recommend a game controller.

iOS 15.0+iPadOS 15.0+visionOS 1.0+

## Details 

Type  

object

## Discussion

Add this key to your information property list if your app requires a game controller in visionOS or to recommend a game controller in iOS. Adding this key requires you to enable the Game Controllers capability in Xcode and ExtendedGamepad under the Game Controllers capability. Xcode sets the value of GCSupportsControllerUserInteraction to `YES` and includes an entry in the GCSupportedGameControllers dictionary with ProfileName set to ExtendedGamepad.

If your app requires a game controller for input in visionOS, add visionOS to the GCRequiresControllerUserInteraction dictionary and set the value to `YES`. If the value is `YES`, the App Store adds a Controller Required badge to your app.

To recommend a game controller in iOS, add iOS to the dictionary and set the value to `YES`. If the value is `YES`, the App Store adds a Controller Recommended badge to your app.

For apps built for visionOS, use only a visionOS platform key in the dictionary. For iOS apps, you can include iOS or visionOS platform keys to indicate behavior in iOS or a compatible iPad or iPhone app running in visionOS.

Important

If your app doesn’t provide an alternate to the game controller for input in visionOS then you need to include an entry in the GCRequiresControllerUserInteraction dictionary and set the value to `YES`.

## Topics

### Platforms

iOS

A Boolean value you use to indicate that a game controller is recommended on iOS.

visionOS

A Boolean value you use to indicate that a game controller is required on visionOS.

## See Also

### Games

AVGameBypassSystemSpatialAudio

A key that ignores the system spatial-audio toggle in Control Center.

GKGameCenterBadgingDisabled

A Boolean value indicating whether GameKit can add badges to a turn-based game icon.

GKShowChallengeBanners

A Boolean value that indicates whether GameKit can display challenge banners in a game.

GCSupportedGameControllers

The types of game controller profiles that the app supports or requires.

**Name:** Supported game controller types

GCSupportsControllerUserInteraction

A Boolean value indicating whether the app supports a game controller.

**Name:** Supports Controller User Interaction

GCSupportsMultipleMicroGamepads

A Boolean value indicating whether the physical Apple TV Remote and the Apple TV Remote app operate as separate game controllers.

