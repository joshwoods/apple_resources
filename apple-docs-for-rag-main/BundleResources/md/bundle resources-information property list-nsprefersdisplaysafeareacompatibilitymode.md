

- Bundle Resources
- Information Property List
-  NSPrefersDisplaySafeAreaCompatibilityMode 

Property List Key

# NSPrefersDisplaySafeAreaCompatibilityMode

A Boolean value that indicates whether the app prefers to run in compatibility mode when necessary.

macOS 12.0+

## Details 

Type  

boolean

## Discussion

On Mac computers that include a camera housing in the screen bezel, the system provides a compatibility mode to prevent apps from unintentionally putting content in the region the housing occupies. When this mode is active, the system changes the active area of the display to avoid the camera housing. The new active area ensures your app’s contents are always visible and not obscured by the camera housing. The system activates this compatibility mode when an app that requires it places a window behind the camera housing in the current desktop or full-screen space.

On Mac computers that include a camera housing, the Finder adds a checkbox to your app’s Get Info panel to enable or disable compatibility mode. If your app’s `Info.plist` file includes the NSPrefersDisplaySafeAreaCompatibilityMode key, the Finder doesn’t add that checkbox; instead, it uses the value of the key to determine whether to run your app in compatibility mode. Set the value of the key to true to always run your app in compatibility mode, and set it to false to never run your app in compatibility mode.

After you audit your app and verify that it runs correctly on Mac computers that include a camera housing, add this key to your `Info.plist` file and set its value to false. If you discover issues during your audit, add the key and set its value to true until you’re able to fix those issues.

Note

On Mac computers that include a camera housing in the bezel, the auxiliaryTopLeftArea and auxiliaryTopRightArea properties of NSScreen contain the regions to the left and right of the camera housing. Use those properties and the visibleFrame property to determine where to display your content.

## See Also

### Styling

UIUserInterfaceStyle

The user interface style for the app.

**Name:** User Interface Style

UIViewEdgeAntialiasing

A Boolean value that indicates whether Core Animation layers use antialiasing when drawing a layer that isn’t aligned to pixel boundaries.

**Name:** Renders with edge antialiasing

UIWhitePointAdaptivityStyle

The app’s white-point adaptivity style, enabled on devices with True Tone displays.

**Name:** White Point Adaptivity Style

UIViewGroupOpacity

A Boolean value that indicates whether Core Animation sublayers inherit the opacity of their superlayer.

**Name:** Renders with group opacity

UIRequiresFullScreen

A Boolean value that indicates whether an iPad app is capable of sharing the screen with other apps.

UISupportsFullScreenInAssistiveAccess

A Boolean value that indicates if an iOS or iPadOS app appears as full screen in Assistive Access.

**Name:** Supports full screen in Assistive Access

NSAccentColorName

The name of a color in an asset catalog to use for a target’s global accent color.

NSWidgetBackgroundColorName

The name of a color in an asset catalog to use for a widget’s configuration interface.

