

- Bundle Resources
- Information Property List
-  UILaunchScreens 

Property List Key

# UILaunchScreens

The user interfaces to show while an app launches in response to different URL schemes.

iOS 14.0+iPadOS 14.0+

## Details 

Type  

object

## Discussion

You use this key if your app supports launching in response to one or more URL schemes, and if you want to provide different launch screens for different launch triggers. If you need only one launch screen, use UILaunchScreen instead.

To define launch screens, create an array of dictionaries, each similar to the one you might provide for UILaunchScreen, but with an added UILaunchScreenIdentifier key that uniquely identifies the screen. Store the array as the value for the UILaunchScreenDefinitions key.

To map from URL schemes to a launch screens, create a dictionary of schemes and identifiers, and store it as the value for the UIURLToLaunchScreenAssociations key. Additionally, indicate a default launch screen by setting a value for the UIDefaultLaunchScreen key.

Note

Use this key to configure the user interface during app launch in a way that doesn’t rely on storyboards. If you prefer to use storyboards to define the launch screen, use the UILaunchStoryboards key instead.

## Topics

### Launch Screen Definitions

UILaunchScreenDefinitions

A collection of launch screen configuration dictionaries.

### Associations

UIURLToLaunchScreenAssociations

The mapping of URL schemes to launch screen configurations.

UIDefaultLaunchScreen

The default launch screen configuration.

## See Also

### Launch interface

UILaunchScreen

The user interface to show while an app launches.

UILaunchStoryboardName

The filename of the storyboard from which to generate the app’s launch image.

**Name:** Launch screen interface file base name

UILaunchStoryboards

The launch storyboard to use to generate a launch image when your app opens from a supported scheme.

LSUIPresentationMode

The initial user-interface mode for the app.

**Name:** Application UI Presentation Mode

UILaunchToFullScreenByDefaultOnMac

A Boolean value that indicates whether to launch your iPad app in full-screen mode when running on a Mac.

