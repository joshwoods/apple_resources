

- AppKit
- NSView
-  NSView.FullScreenModeOptionKey 

Structure

# NSView.FullScreenModeOptionKey

These constants are keys that you can use in the options dictionary in enterFullScreenMode(_:withOptions:) and exitFullScreenMode(options:).

macOS

``` source
struct FullScreenModeOptionKey
```

## Topics

### Type Properties

static let fullScreenModeAllScreens: NSView.FullScreenModeOptionKey

Key whose corresponding value specifies whether the view should take over all screens.

static let fullScreenModeApplicationPresentationOptions: NSView.FullScreenModeOptionKey

Key whose corresponding value specifies the application presentation options.

static let fullScreenModeSetting: NSView.FullScreenModeOptionKey

Key whose corresponding value specifies the full screen mode setting.

static let fullScreenModeWindowLevel: NSView.FullScreenModeOptionKey

Key whose corresponding value specifies the screen mode window level.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Drawing the View in Fullscreen Mode

func enterFullScreenMode(NSScreen, withOptions: [NSView.FullScreenModeOptionKey : Any]?) -> Bool

Sets the view to full screen mode.

func exitFullScreenMode(options: [NSView.FullScreenModeOptionKey : Any]?)

Instructs the view to exit full screen mode.

var isInFullScreenMode: Bool

A Boolean value indicating whether the view is in full screen mode.

