

- AppKit
- NSApplication
-  appearance 

Instance Property

# appearance

The appearance associated with the app’s windows.

macOS 10.14+

``` source
@MainActor
var appearance: NSAppearance? { get set }
```

## Mentioned in 

Choosing a Specific Appearance for Your macOS App

## Discussion

When the value of this property is `nil` (the default), AppKit applies the current system appearance to the app’s user interface elements, including its windows, views, panels, and popovers. Assigning an NSAppearance object to this property causes the app’s interface elements to adopt the specified appearance instead.

Individual windows and views may still override the app’s appearance to customize their own appearance.

## See Also

### Managing the App’s Appearance

var effectiveAppearance: NSAppearance

The appearance that AppKit uses to draw the app’s interface.

var currentSystemPresentationOptions: NSApplication.PresentationOptions

The set of app presentation options that are currently in effect for the system.

var presentationOptions: NSApplication.PresentationOptions

The presentation options that should be in effect for the system when this app is active.

struct PresentationOptions

Constants that control the presentation of the app, typically for fullscreen apps such as games or kiosks.

