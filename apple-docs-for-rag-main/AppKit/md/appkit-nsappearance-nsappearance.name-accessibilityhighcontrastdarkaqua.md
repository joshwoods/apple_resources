

- AppKit
- NSAppearance
- NSAppearance.Name
-  accessibilityHighContrastDarkAqua 

Type Property

# accessibilityHighContrastDarkAqua

A high-contrast version of the standard dark system appearance.

macOS 10.14+

``` source
static let accessibilityHighContrastDarkAqua: NSAppearance.Name
```

## Discussion

Don’t assign an NSAppearance object with this type directly to one of your views. Instead, assign a dark appearance to your view. AppKit then returns this type when the user enables the Increase Contrast option in the Accessibility system preferences.

## See Also

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

static let accessibilityHighContrastVibrantLight: NSAppearance.Name

A high-contrast version of the light vibrant appearance.

static let accessibilityHighContrastVibrantDark: NSAppearance.Name

A high-contrast version of the dark vibrant appearance.

