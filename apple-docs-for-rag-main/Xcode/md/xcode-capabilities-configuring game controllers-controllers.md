

- Xcode
- Capabilities
-  Configuring game controllers 

Article

# Configuring game controllers

Enhance gameplay input by enabling the discovery, configuration, and use of physical game controllers.

## Overview

Game controllers provide physical controls to trigger actions in your game. Apple specifies the look and behavior of the controls to MFi accessory manufacturers, which means you can rely on a consistent set of high-quality controls in all supported game controllers.

A game that supports game controllers enables one or more different *game-controller profiles* — objects that map physical controls on a device to the inputs your game requires — such as Extended, Micro, and Directional. The game also specifies the preferred order of use for these profiles. After retrieving a profile from the connected game controller, your game periodically requests the device’s current values or installs handlers that the system invokes when those values change.

Before you can select the profiles your game supports, follow the steps in Add a capability to add the Game Controllers capability to your game’s target.

After you add the Game Controllers capability to your game’s target, Xcode appends the GCSupportsControllerUserInteraction key to its `Info.plist` file with a value of `true` to indicate to the system that your game supports game controllers.

Note

The Game Controllers capability is only available to games that target iOS, iPadOS, tvOS, and visionOS.

### Select the supported game controller profiles

When you add support for game controllers to your app, you don’t integrate with specific hardware. Instead, you integrate one or more of the game-controller profiles that the Game Controller framework provides. Each profile maps to a control layout that Apple defines, and that profile describes a set of physical controls that the hardware manufacturer guarantees to be available on the controller.

To indicate to the system which game-controller profiles your game supports, perform the following steps:

1.  Select your project in Xcode’s Project navigator.

2.  Select the game’s target from the Targets list.

3.  Click the Signing & Capabilities tab in the project editor.

4.  Find the Game Controllers capability.

5.  Select the appropriate game controller profiles by checking their checkboxes.

Xcode adds the GCSupportedGameControllers array to your game’s `Info.plist` file, if it’s not already present, and populates it with names of the selected game-controller profiles. For more information about each profile, see GCExtendedGamepad, GCMicroGamepad, and GCDirectionalGamepad.

Hardware controllers can support multiple profiles; if you enable more than one game controller profile, drag the profiles and arrange them in your preferred order. For example, if your game supports both the Extended and Micro profiles, but optimizes gameplay for the Micro profile, place that profile at the top of the list.

For more information, see the video Tap into virtual and physical game controllers and the sample code Supporting Game Controllers.

## See Also

### App execution

Configuring background execution modes

Indicate the background services your app requires to continue executing in the background in iOS, iPadOS, tvOS, visionOS, and watchOS.

Configuring custom fonts

Register your app as a provider or consumer of systemwide custom fonts.

Configuring Maps support

Register your iOS routing app to provide point-to-point directions to Maps and other apps.

Configuring Siri support

Enable your app and its Intents extension to resolve, confirm, and handle user-driven Siri requests for your app’s services.

