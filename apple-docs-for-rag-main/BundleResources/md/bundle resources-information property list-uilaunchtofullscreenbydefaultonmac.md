

- Bundle Resources
- Information Property List
-  UILaunchToFullScreenByDefaultOnMac 

Property List Key

# UILaunchToFullScreenByDefaultOnMac

A Boolean value that indicates whether to launch your iPad app in full-screen mode when running on a Mac.

macOS 12.1+

## Details 

Type  

boolean

## Discussion

To launch your iPad app in full-screen mode when running in macOS, add this key to your app’s `Info.plist` file and set its value to true. State restoration can override this behavior if the person using your app exits full-screen mode before quitting the app.

You can also provide a pixel-perfect, edge-to-edge, full-screen experience by including the UISupportsTrueScreenSizeOnMac key with a value of true in your app’s `Info.plist` file.

UILaunchToFullScreenByDefaultOnMac has no effect on your iPad app when:

- The app supports iPad multitasking and resizable windows. For more information, see UIRequiresFullScreen.

- The app is running on other Apple platforms.

- The app is built with Mac Catalyst.

## See Also

### Launch interface

UILaunchScreen

The user interface to show while an app launches.

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

