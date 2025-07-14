

- Bundle Resources
- Information Property List
-  UILaunchScreen 

Property List Key

# UILaunchScreen

The user interface to show while an app launches.

iOS 14.0+iPadOS 14.0+

## Details 

Type  

object

## Discussion

You use this key to define the launch screen that the system displays while your app launches. If you need to provide different launch screens in response to being launched by different URL schemes, use UILaunchScreens instead.

Note

Use this key to configure the user interface during app launch in a way that doesn’t rely on storyboards. If you prefer to use storyboards, use UILaunchStoryboardName instead.

## Topics

### Main Interface

UIColorName

The name of a color to use as the background color on the launch screen.

UIImageName

The name of an image to display during app launch.

UIImageRespectsSafeAreaInsets

A Boolean that specifies whether the launch image should respect the safe area insets.

### Border Elements

UINavigationBar

Navigation bar visibility and configuration during launch.

UITabBar

Tab bar visibility and configuration during launch.

UIToolbar

Toolbar visibility and configuration during launch.

## See Also

### Launch interface

UILaunchScreens

The user interfaces to show while an app launches in response to different URL schemes.

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

