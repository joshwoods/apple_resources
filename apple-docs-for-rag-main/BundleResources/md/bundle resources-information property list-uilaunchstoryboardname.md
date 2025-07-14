

- Bundle Resources
- Information Property List
-  UILaunchStoryboardName 

Property List Key

# UILaunchStoryboardName

The filename of the storyboard from which to generate the app’s launch image.

iOS 9.0+iPadOS 9.0+tvOS 9.0+watchOS 2.0+

## Details 

Name  
Launch screen interface file base name

Type  

string

## Discussion

Specify the name of the storyboard file without the filename extension. For example, if the filename of your storyboard is `LaunchScreen.storyboard`, specify “LaunchScreen” as the value for this key.

If you prefer to configure your app’s launch screen without storyboards, use UILaunchScreen instead.

## See Also

### Launch interface

UILaunchScreen

The user interface to show while an app launches.

UILaunchScreens

The user interfaces to show while an app launches in response to different URL schemes.

UILaunchStoryboards

The launch storyboard to use to generate a launch image when your app opens from a supported scheme.

LSUIPresentationMode

The initial user-interface mode for the app.

**Name:** Application UI Presentation Mode

UILaunchToFullScreenByDefaultOnMac

A Boolean value that indicates whether to launch your iPad app in full-screen mode when running on a Mac.

