

- Bundle Resources
- Information Property List
-  UISupportsTrueScreenSizeOnMac 

Property List Key

# UISupportsTrueScreenSizeOnMac

A Boolean value that indicates whether your iPad app supports arbitrary screen sizes and resolutions when running on a Mac.

macOS 12.1+

## Details 

Type  

boolean

## Discussion

To declare support for arbitrary screen sizes and resolutions when running your iPad app in macOS, add this key to your app’s `Info.plist` file and set its value to true. This key has no effect when:

- The app supports iPad multitasking and resizable windows. For more information, see UIRequiresFullScreen.

- The app is running on other Apple platforms.

- The app is built with Mac Catalyst.

The use of this key implies that your app is capable of handling a variety of display configurations available on a Mac, including:

- Small to large display resolutions; for example, 640 x 480 to 8K and beyond.

- Retina and non-Retina displays.

- All conceivable aspect ratios, including portrait and 21:9 ultrawide.

Use of the UISupportsTrueScreenSizeOnMac key also implies that your app is capable of handling portrait and landscape sizes even when they don’t align with the device orientation. For instance, if your app supports rotation in iPadOS, the device orientation is always landscape even though the display might have a portrait aspect ratio in reality.

Note

When running your iPad app on a Mac, macOS chooses the device orientation of your app from the set of app-supported orientations for iOS, regardless of the actual Mac display aspect ratio. This means that you don’t need to update the set of iOS-supported orientations (see UISupportedInterfaceOrientations), or alter your code to handle unsupported orientations when using the UISupportsTrueScreenSizeOnMac key.

When you include UISupportsTrueScreenSizeOnMac in your app, your app is responsible for:

- Handling memory management concerns that may occur when running at extreme resolutions.

- Handling layout concerns for different aspect ratios, such as correct button placement.

- Letterboxing and pillarboxing as needed if your app requires a specific aspect ratio.

To provide a pixel-perfect, edge-to-edge, full-screen experience, use UISupportsTrueScreenSizeOnMac along with the UILaunchToFullScreenByDefaultOnMac key.

## See Also

### Main user interface

UIApplicationSceneManifest

The information about the app’s scene-based life-cycle support.

**Name:** Application Scene Manifest

UIApplicationPreferredDefaultSceneSessionRole

The preferred initial scene session role for your app.

NSMainStoryboardFile

The name of an app’s storyboard resource file.

**Name:** Main storyboard file base name

UIMainStoryboardFile

The name of the app’s main storyboard file.

**Name:** Main storyboard file base name

NSMainNibFile

The name of an app’s main user interface file.

**Name:** Main nib file base name

LSUIElement

A Boolean value indicating whether the app is an agent app that runs in the background and doesn’t appear in the Dock.

**Name:** Application is agent (UIElement)

