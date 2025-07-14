

- Bundle Resources
- Information Property List
-  AVGameBypassSystemSpatialAudio 

Property List Key

# AVGameBypassSystemSpatialAudio

A key that ignores the system spatial-audio toggle in Control Center.

iOS 18.0+iPadOS 18.0+tvOS 18.0+

## Details 

Type  

boolean

## Discussion

In iOS 18 and tvOS 18 and later, the system automatically adds spatial audio to the output for games. To opt out of automatic spatial audio and support just your preferred spatial audio setup, add this key to your app’s `Info.plist`.

## See Also

### Games

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

GCRequiresControllerUserInteraction

The platforms for which your app requires or you recommend a game controller.

GCSupportsMultipleMicroGamepads

A Boolean value indicating whether the physical Apple TV Remote and the Apple TV Remote app operate as separate game controllers.

