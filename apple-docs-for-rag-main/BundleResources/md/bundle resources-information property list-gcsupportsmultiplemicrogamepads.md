

- Bundle Resources
- Information Property List
-  GCSupportsMultipleMicroGamepads 

Property List Key

# GCSupportsMultipleMicroGamepads

A Boolean value indicating whether the physical Apple TV Remote and the Apple TV Remote app operate as separate game controllers.

tvOS 9.0+

## Details 

Type  

boolean

## Discussion

If set to `YES`, your app supports multiple remotes with gamepads; otherwise, it doesn’t. If you support the 2nd Generation Siri Remote, set this key to `YES`. If you don’t set this key to `YES`, the combined micro gamepads won’t have the extra inputs of the 2nd Generation Siri Remote.

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

GCRequiresControllerUserInteraction

The platforms for which your app requires or you recommend a game controller.

