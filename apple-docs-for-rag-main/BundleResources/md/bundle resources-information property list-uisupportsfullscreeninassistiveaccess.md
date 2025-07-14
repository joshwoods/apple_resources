

- Bundle Resources
- Information Property List
-  UISupportsFullScreenInAssistiveAccess 

Property List Key

# UISupportsFullScreenInAssistiveAccess

A Boolean value that indicates if an iOS or iPadOS app appears as full screen in Assistive Access.

iOS 17.0+iPadOS 17.0+

## Details 

Name  
Supports full screen in Assistive Access

Type  

boolean

## Attributes 

Default: `YES`

## Discussion

Adding this key to your app’s `Info.plist` file with a value of `YES` allows your app’s UI to expand into all the available space above the Back button in Assistive Access. It also lists your app as Optimized for Assistive Access in Settings, so that a trusted supporter configuring Assistive Access on someone’s behalf knows that your app’s UI is optimized for this feature.

For more information, read Optimizing your app for Assistive Access.

## See Also

### Related Documentation

Assistive Access

A mode that tailors the iOS and iPadOS experience for people with cognitive disabilities.

Optimizing your app for Assistive Access

Adjust your app’s UI to make sure it works well for people who use Assistive Access.

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

NSPrefersDisplaySafeAreaCompatibilityMode

A Boolean value that indicates whether the app prefers to run in compatibility mode when necessary.

NSAccentColorName

The name of a color in an asset catalog to use for a target’s global accent color.

NSWidgetBackgroundColorName

The name of a color in an asset catalog to use for a widget’s configuration interface.

