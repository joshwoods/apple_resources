

- Bundle Resources
- Information Property List
-  UIRequiresFullScreen 

Property List Key

# UIRequiresFullScreen

A Boolean value that indicates whether an iPad app is capable of sharing the screen with other apps.

iOS 9.0+iPadOS 9.0+

## Details 

Type  

boolean

## Discussion

iPad multitasking lets multiple apps appear on screen at the same time. Dragging the resize controls causes the system to change the size of each app’s window. Each app must then adjust its content to fit the newly available space.

If your app’s content requires a full-screen presentation, include this key in your `Info.plist` and set its value to true. When you do, the system prevents your app from sharing the screen with other apps. On an external screen, the window for an app with this setting maintains its canvas size.

Don’t include this key in your `Info.plist` file if your app supports iPad multitasking and is capable of running alongside other apps. To take advantage of the full size of an external screen consider adopting resizability and multitasking support. If this key is absent, or is present and set to false, the system lets your app share the screen with other apps.

## See Also

### Related Documentation

Multitasking on iPad

Implement multitasking APIs to seamlessly integrate your app with iPadOS.

Presenting content on a connected display

Fill connected displays with additional content from your app.

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

UISupportsFullScreenInAssistiveAccess

A Boolean value that indicates if an iOS or iPadOS app appears as full screen in Assistive Access.

**Name:** Supports full screen in Assistive Access

NSPrefersDisplaySafeAreaCompatibilityMode

A Boolean value that indicates whether the app prefers to run in compatibility mode when necessary.

NSAccentColorName

The name of a color in an asset catalog to use for a target’s global accent color.

NSWidgetBackgroundColorName

The name of a color in an asset catalog to use for a widget’s configuration interface.

