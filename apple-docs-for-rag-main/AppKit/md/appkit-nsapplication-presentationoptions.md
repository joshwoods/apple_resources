

- AppKit
- NSApplication
-  presentationOptions 

Instance Property

# presentationOptions

The presentation options that should be in effect for the system when this app is active.

macOS 10.6+

``` source
@MainActor
var presentationOptions: NSApplication.PresentationOptions { get set }
```

## Discussion

This value contains a bitwise OR of the constants listed in NSApplication.PresentationOptions. Trying to set the property to an invalid combination of option flags raises an invalidArgumentException exception. See the constants for a description of the valid combinations.

## See Also

### Managing the App’s Appearance

var appearance: NSAppearance?

The appearance associated with the app’s windows.

var effectiveAppearance: NSAppearance

The appearance that AppKit uses to draw the app’s interface.

var currentSystemPresentationOptions: NSApplication.PresentationOptions

The set of app presentation options that are currently in effect for the system.

struct PresentationOptions

Constants that control the presentation of the app, typically for fullscreen apps such as games or kiosks.

