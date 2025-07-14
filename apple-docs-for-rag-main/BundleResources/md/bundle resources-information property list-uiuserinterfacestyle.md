

- Bundle Resources
- Information Property List
-  UIUserInterfaceStyle 

Property List Key

# UIUserInterfaceStyle

The user interface style for the app.

iOS 13.0+iPadOS 13.0+tvOS 10.0+

## Details 

Name  
User Interface Style

Type  

string

## Possible Values 

`Automatic`  

Set this value to adopt the systemwide user interface style, and observe any changes to that style. This is the default value, and provides the same functionality as if the key weren’t explicitly set.

`Light`  

Set this value to force the light user interface style, even when the systemwide style is set to dark. Your app will ignore any changes to the systemwide style.

`Dark`  

Set this value to force the dark user interface style, even when the systemwide style is set to light. Your app will ignore any changes to the systemwide style.

## Attributes 

Default: `Automatic`

## See Also

### Styling

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

NSWidgetBackgroundColorName

The name of a color in an asset catalog to use for a widget’s configuration interface.

