

- Bundle Resources
- Information Property List
-  NSWidgetBackgroundColorName 

Property List Key

# NSWidgetBackgroundColorName

The name of a color in an asset catalog to use for a widget’s configuration interface.

iOS 14.0+iPadOS 14.0+macOS 11.0+

## Details 

Type  

string

## Discussion

This `Info.plist` value controls the background color shown in the widget configuration interface while editing a widget.

While you can set this directly in your Info.plist, the recommended approach is to use the `Widget Background Color Name` build setting (in the `Asset Catalog Compiler - Options` section) of the widget extension target. Set the value of the build setting to the name of the Color Set in the asset catalog. Xcode automatically sets `NSWidgetBackgroundColorName` to the appropriate value in the `Info.plist` file when building your project.

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

NSPrefersDisplaySafeAreaCompatibilityMode

A Boolean value that indicates whether the app prefers to run in compatibility mode when necessary.

NSAccentColorName

The name of a color in an asset catalog to use for a target’s global accent color.

