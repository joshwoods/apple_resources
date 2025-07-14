

- Updates
-  Game Controller updates 

Article

# Game Controller updates

Learn about important changes to Game Controller.

## Overview

Browse notable changes in Game Controller.

## June 2024

### visionOS

- For UIKit apps, add a user interaction that determines whether the system delivers game controller events through the Game Controller framework instead of the UIResponder chain. To receive events through the Game Controller framework, add a GCEventInteraction object to one or more views and set the handledEventTypes property to the types of events you want to handle.

## June 2023

- Use the classes that conform to the GCDevicePhysicalInput protocol to poll for game controller input in your game loop. For more information, see Handling input events.

- Add support for arcade sticks. To determine if a controller is an arcade stick, check whether the product category is GCProductCategoryArcadeStick.

- Add GCRequiresControllerUserInteraction to your information property list if your app requires a game controller on visionOS or to recommend a game controller on iOS.

## See Also

### Technology updates

Accelerate updates

Learn about important changes to Accelerate.

Accessibility updates

Learn about important changes to Accessibility.

ActivityKit updates

Learn about important changes in ActivityKit.

AdAttributionKit Updates

Learn about important changes to AdAttributionKit.

App Intents updates

Learn about important changes in App Intents.

AppKit updates

Learn about important changes to AppKit.

Apple Intelligence updates

Learn about important changes to Apple Intelligence.

Apple Pencil updates

Learn about important changes to Apple Pencil.

ARKit updates

Learn about important changes to ARKit.

Audio Toolbox updates

Learn about important changes to Audio Toolbox.

AuthenticationServices updates

Learn about important changes to AuthenticationServices.

AVFAudio updates

Learn about important changes to AVFAudio.

AVFoundation updates

Learn about important changes to AVFoundation.

Bundle Resources updates

Learn about important changes to Bundle Resources.

ContactsUI updates

Learn about important changes to ContactsUI.

