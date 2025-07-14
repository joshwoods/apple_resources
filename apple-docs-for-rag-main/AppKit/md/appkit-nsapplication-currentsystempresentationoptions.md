

- AppKit
- NSApplication
-  currentSystemPresentationOptions 

Instance Property

# currentSystemPresentationOptions

The set of app presentation options that are currently in effect for the system.

macOS 10.6+

``` source
@MainActor
var currentSystemPresentationOptions: NSApplication.PresentationOptions { get }
```

## Return Value

The presentation options. The constants are listed in NSApplication.PresentationOptions and can combined using a C bitwise OR operator.

## Discussion

This property contains the presentation options that have been put into effect by the currently active app. You can use key-value observing on this property to receive notifications when:

- The client is the active app and makes a change itself using either the presentationOptions property or the `SetSystemUIMode` function.

- Another app is active and makes presentation changes of its own.

- Another app becomes active and causes the active set of presentation options to change.

Key-value observing notifications aren’t sent when one of the above conditions occur, but has the same set of presentation options as the previously active app.

## See Also

### Managing the App’s Appearance

var appearance: NSAppearance?

The appearance associated with the app’s windows.

var effectiveAppearance: NSAppearance

The appearance that AppKit uses to draw the app’s interface.

var presentationOptions: NSApplication.PresentationOptions

The presentation options that should be in effect for the system when this app is active.

struct PresentationOptions

Constants that control the presentation of the app, typically for fullscreen apps such as games or kiosks.

