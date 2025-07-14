

- SwiftUI
- Color
-  accentColor 

Type Property

# accentColor

A color that reflects the accent color of the system or app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static var accentColor: Color { get }
```

## Discussion

The accent color is a broad theme color applied to views and controls. You can set it at the application level by specifying an accent color in your app’s asset catalog.

Note

In macOS, SwiftUI applies customization of the accent color only if the user chooses Multicolor under General \> Accent color in System Preferences.

The following code renders a Text view using the app’s accent color:

```
Text("Accent Color")
    .foregroundStyle(Color.accentColor)
```

## See Also

### Getting semantic colors

static let primary: Color

The color to use for primary content.

static let secondary: Color

The color to use for secondary content.

