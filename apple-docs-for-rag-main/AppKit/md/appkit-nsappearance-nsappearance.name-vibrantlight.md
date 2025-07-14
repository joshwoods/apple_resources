

- AppKit
- NSAppearance
- NSAppearance.Name
-  vibrantLight 

Type Property

# vibrantLight

The light vibrant appearance, available only in visual effect views.

macOS 10.10+

``` source
static let vibrantLight: NSAppearance.Name
```

## Discussion

Vibrant appearances use color blending to make the foreground appearance stand out from the background more prominently.

Don’t assign an NSAppearance object with this type directly to one of your views. Instead, assign a light appearance to your view, make sure its allowsVibrancy property is set to true, and embed the view in a visual effect view. When you do, AppKit updates your view’s appearance to this type.

## See Also

### System Appearance Names

static let aqua: NSAppearance.Name

The standard light system appearance.

static let darkAqua: NSAppearance.Name

The standard dark system appearance.

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

