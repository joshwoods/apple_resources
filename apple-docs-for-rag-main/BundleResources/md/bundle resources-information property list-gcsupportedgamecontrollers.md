

- Bundle Resources
- Information Property List
-  GCSupportedGameControllers 

Property List Key

# GCSupportedGameControllers

The types of game controller profiles that the app supports or requires.

iOS 7.0+iPadOS 7.0+macOS 10.9+tvOS 9.0+visionOS 1.0+

## Details 

Name  
Supported game controller types

Type  

array of dictionaries

## Properties

`ProfileName`

`string`

Possible Values: `DirectionalGamepad, ExtendedGamepad, MicroGamepad`

## Discussion

The dictionary keys are `ProfileName` and the possible game controller values are:

`ExtendedGamepad`  
The extended set of gamepad controls. See GCExtendedGamepad.

`MicroGamepad`  
The 1st Generation Siri Remote. See GCMicroGamepad.

`DirectionalGamepad`  
The 2nd Generation Siri Remote. A directional pad without motion or rotation. See GCDirectionalGamepad. Available in iOS 14.3+, macOS 11.1+, Mac Catalyst 14.3+, and tvOS 14.3+.

## See Also

### Games

AVGameBypassSystemSpatialAudio

A key that ignores the system spatial-audio toggle in Control Center.

GKGameCenterBadgingDisabled

A Boolean value indicating whether GameKit can add badges to a turn-based game icon.

GKShowChallengeBanners

A Boolean value that indicates whether GameKit can display challenge banners in a game.

GCSupportsControllerUserInteraction

A Boolean value indicating whether the app supports a game controller.

**Name:** Supports Controller User Interaction

GCRequiresControllerUserInteraction

The platforms for which your app requires or you recommend a game controller.

GCSupportsMultipleMicroGamepads

A Boolean value indicating whether the physical Apple TV Remote and the Apple TV Remote app operate as separate game controllers.

