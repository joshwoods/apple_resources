

- AppKit
- NSAppearance
-  NSAppearance.Name 

Structure

# NSAppearance.Name

macOS

``` source
struct Name
```

## Topics

### System Appearance Names

static let aqua: NSAppearance.Name

The standard light system appearance.

static let darkAqua: NSAppearance.Name

The standard dark system appearance.

static let vibrantLight: NSAppearance.Name

The light vibrant appearance, available only in visual effect views.

static let vibrantDark: NSAppearance.Name

A dark vibrant appearance, available only in visual effect views.

static let accessibilityHighContrastAqua: NSAppearance.Name

A high-contrast version of the standard light system appearance.

static let accessibilityHighContrastDarkAqua: NSAppearance.Name

A high-contrast version of the standard dark system appearance.

static let accessibilityHighContrastVibrantLight: NSAppearance.Name

A high-contrast version of the light vibrant appearance.

static let accessibilityHighContrastVibrantDark: NSAppearance.Name

A high-contrast version of the dark vibrant appearance.

### Deprecated Appearance Names

static let lightContent: NSAppearance.Name

The standard appearance that can be used by controls in light content areas (not including window-frame areas).

Deprecated

### Initializers

init(String)

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Appearance Name

var name: NSAppearance.Name

The name of the appearance.

