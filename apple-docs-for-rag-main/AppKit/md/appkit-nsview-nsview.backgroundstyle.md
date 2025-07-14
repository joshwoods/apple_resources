

- AppKit
- NSView
-  NSView.BackgroundStyle 

Enumeration

# NSView.BackgroundStyle

Background styles to apply to a view’s cell.

macOS 10.5+

``` source
enum BackgroundStyle
```

## Overview

Apply these styles to the backgroundStyle or interiorBackgroundStyle properties of an NSCell object.

## Topics

### Getting the Background Styles

case normal

A style that reflects the predominant color scheme of the view’s appearance.

case emphasized

A style that adds emphasis to the background using an alternate color or visual effect.

case raised

A style that makes the background appear higher than the content drawn on it.

case lowered

A style that makes the background appear lower than the content drawn on it.

### Deprecated

static let light: NSView.BackgroundStyle

The background is a light color.

Deprecated

static let dark: NSView.BackgroundStyle

The background is a dark color.

Deprecated

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Display Attributes

var isBezeled: Bool

A Boolean value indicating whether the cell has a bezeled border.

var isBordered: Bool

A Boolean value indicating whether the cell draws itself outlined with a plain border.

var isOpaque: Bool

A Boolean value indicating whether the cell is completely opaque.

var controlTint: NSControlTint

The cell’s control tint.

Deprecated

var backgroundStyle: NSView.BackgroundStyle

The cell’s background style.

var interiorBackgroundStyle: NSView.BackgroundStyle

The cell’s interior background style.

