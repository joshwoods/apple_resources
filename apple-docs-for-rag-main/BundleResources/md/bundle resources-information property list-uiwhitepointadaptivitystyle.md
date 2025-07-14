

- Bundle Resources
- Information Property List
-  UIWhitePointAdaptivityStyle 

Property List Key

# UIWhitePointAdaptivityStyle

The app’s white-point adaptivity style, enabled on devices with True Tone displays.

iOS 9.3+iPadOS 9.3+

## Details 

Name  
White Point Adaptivity Style

Type  

string

## Possible Values 

`UIWhitePointAdaptivityStyleStandard`  

The default white-point adaptivity.

`UIWhitePointAdaptivityStyleReading`  

A stronger adaptivity style designed for reading-focused apps.

`UIWhitePointAdaptivityStylePhoto`  

A weaker adaptivity style designed for photography-focused apps.

`UIWhitePointAdaptivityStyleVideo`  

A weaker adaptivity style designed for video-focused apps.

`UIWhitePointAdaptivityStyleGame`  

A weaker adaptifity style designed for games.

## Attributes 

Default: `UIWhitePointAdaptivityStyleStandard`

## Discussion

In split view, the system applies the style on the entire screen from the app with the weaker adaptivity style setting. For example, if one app uses the `UIWhitePointAdaptivityStylePhoto` style and another uses the `UIWhitePointAdaptivityStyleReading` style, the system uses the weaker `UIWhitePointAdaptivityStyleReading` style for the entire screen.

## See Also

### Styling

UIUserInterfaceStyle

The user interface style for the app.

**Name:** User Interface Style

UIViewEdgeAntialiasing

A Boolean value that indicates whether Core Animation layers use antialiasing when drawing a layer that isn’t aligned to pixel boundaries.

**Name:** Renders with edge antialiasing

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

NSWidgetBackgroundColorName

The name of a color in an asset catalog to use for a widget’s configuration interface.

