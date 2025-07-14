

- Bundle Resources
- Information Property List
-  UILaunchStoryboards 

Property List Key

# UILaunchStoryboards

The launch storyboard to use to generate a launch image when your app opens from a supported scheme.

iOS 9.0+iPadOS 9.0+

## Details 

Type  

object

## Discussion

Use UILaunchStoryboards when you want your app to show a different launch screen for different schemes. The schemes are the ones specified in your app’s CFBundleURLTypes. You can also specify a default launch storyboard.

If your app has a single launch storyboard, use the simpler UILaunchStoryboardName instead.

## Topics

### Specifying Launch Storyboards

UILaunchStoryboardDefinitions

An array of dictionaries mapping launch storyboard identifiers to storyboards.

UIDefaultLaunchStoryboard

The identifier of the default launch storyboard to use.

### Associating Storyboard Identifiers with Schemes

UIURLToLaunchStoryboardAssociations

The user-defined storyboard identifiers that associate with supported schemes.

## See Also

### Launch interface

UILaunchScreen

The user interface to show while an app launches.

UILaunchScreens

The user interfaces to show while an app launches in response to different URL schemes.

UILaunchStoryboardName

The filename of the storyboard from which to generate the app’s launch image.

**Name:** Launch screen interface file base name

LSUIPresentationMode

The initial user-interface mode for the app.

**Name:** Application UI Presentation Mode

UILaunchToFullScreenByDefaultOnMac

A Boolean value that indicates whether to launch your iPad app in full-screen mode when running on a Mac.

