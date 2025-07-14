

- AppKit
- NSApplication
-  effectiveAppearance 

Instance Property

# effectiveAppearance

The appearance that AppKit uses to draw the app’s interface.

macOS 10.14+

``` source
@MainActor
var effectiveAppearance: NSAppearance { get }
```

## Discussion

This property always contains an NSAppearance object representing the appearance to use during drawing. If you don’t explicitly assign a value to the appearance property, the app inherits the system’s effective appearance.

## See Also

### Managing the App’s Appearance

var appearance: NSAppearance?

The appearance associated with the app’s windows.

var currentSystemPresentationOptions: NSApplication.PresentationOptions

The set of app presentation options that are currently in effect for the system.

var presentationOptions: NSApplication.PresentationOptions

The presentation options that should be in effect for the system when this app is active.

struct PresentationOptions

Constants that control the presentation of the app, typically for fullscreen apps such as games or kiosks.

