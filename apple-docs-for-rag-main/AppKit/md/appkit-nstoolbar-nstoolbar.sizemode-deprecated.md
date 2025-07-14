

- AppKit
- NSToolbar
-  NSToolbar.SizeMode Deprecated

Enumeration

# NSToolbar.SizeMode

Constants that specify toolbar display modes.

Mac Catalyst 13.1+macOS 10.0–15.4Deprecated

``` source
enum SizeMode
```

Deprecated

The toolbar no longer uses this type.

## Topics

### Constants

case `default`

The toolbar uses the system-defined default size, which is `NSToolbarSizeModeRegular`.

case regular

The toolbar uses regular-sized controls and 32 by 32 pixel icons.

case small

The toolbar uses small-sized controls and 24 by 24 pixel icons.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Deprecated

var centeredItemIdentifier: NSToolbarItem.Identifier?

The item to display in the center of the toolbar.

Deprecated

var fullScreenAccessoryView: NSView?

The toolbar’s full screen accessory view.

Deprecated

var fullScreenAccessoryViewMinHeight: CGFloat

The minimum height of the toolbar’s full screen accessory view.

Deprecated

var fullScreenAccessoryViewMaxHeight: CGFloat

The maximum height of the toolbar’s full screen accessory view, in points.

Deprecated

var sizeMode: NSToolbar.SizeMode

The toolbar’s size mode.

Deprecated

