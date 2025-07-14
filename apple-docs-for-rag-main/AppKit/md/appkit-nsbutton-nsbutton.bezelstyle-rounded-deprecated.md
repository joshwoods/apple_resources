

- AppKit
- NSButton
- NSButton.BezelStyle
-  rounded Deprecated

Type Property

# rounded

A rounded rectangle button, designed for text.

macOS 10.0–15.4Deprecated

``` source
static var rounded: NSButton.BezelStyle { get }
```

## Discussion

Rounded buttons are common within the body of a window or alert. To configure a button as the default button, set the keyEquivalent property to the carriage return character (`\r`, ASCII `0xd`). The system draws the default button prominently using the accent color to indicate that the user can press the return key to invoke the button’s action.

## See Also

### Properties

static var inline: NSButton.BezelStyle

A button that has a solid round-rectangle border background.

Deprecated

static var recessed: NSButton.BezelStyle

A bezel style appropriate for use in scope bars and title bar accessories, similar to the bookmarks bar in Safari.

Deprecated

static var regularSquare: NSButton.BezelStyle

A rectangular button with a two-point border, designed for icons.

Deprecated

static var roundedDisclosure: NSButton.BezelStyle

A bezel style for use with a vertically expanding and collapsing disclosure button.

Deprecated

static var roundRect: NSButton.BezelStyle

A bezel style appropriate for use as an action or auxiliary button in scope bars and title bar accessories.

Deprecated

static var texturedRounded: NSButton.BezelStyle

A bezel style appropriate for use in the toolbar or title bar regions of a window.

Deprecated

