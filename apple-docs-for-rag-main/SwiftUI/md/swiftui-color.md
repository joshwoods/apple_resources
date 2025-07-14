

- SwiftUI
-  Color 

Structure

# Color

A representation of a color that adapts to a given context.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct Color
```

## Mentioned in 

Laying out a simple view

## Overview

You can create a color in one of several ways:

- Load a color from an Asset Catalog:

  ```
  let aqua = Color("aqua") // Looks in your app's main bundle by default.
  ```

- Specify component values, like red, green, and blue; hue, saturation, and brightness; or white level:

  ```
  let skyBlue = Color(red: 0.4627, green: 0.8392, blue: 1.0)
  let lemonYellow = Color(hue: 0.1639, saturation: 1, brightness: 1)
  let steelGray = Color(white: 0.4745)
  ```

- Create a color instance from another color, like a UIColor or an NSColor:

  ```
  #if os(iOS)
  let linkColor = Color(uiColor: .link)
  #elseif os(macOS)
  let linkColor = Color(nsColor: .linkColor)
  #endif
  ```

- Use one of a palette of predefined colors, like black, green, and purple.

Some view modifiers can take a color as an argument. For example, foregroundStyle(_:) uses the color you provide to set the foreground color for view elements, like text or SF Symbols:

```
Image(systemName: "leaf.fill")
    .foregroundStyle(Color.green)
```

Because SwiftUI treats colors as View instances, you can also directly add them to a view hierarchy. For example, you can layer a rectangle beneath a sun image using colors defined above:

```
ZStack {
    skyBlue
    Image(systemName: "sun.max.fill")
        .foregroundStyle(lemonYellow)
}
.frame(width: 200, height: 100)
```

A color used as a view expands to fill all the space it’s given, as defined by the frame of the enclosing ZStack in the above example:

SwiftUI only resolves a color to a concrete value just before using it in a given environment. This enables a context-dependent appearance for system defined colors, or those that you load from an Asset Catalog. For example, a color can have distinct light and dark variants that the system chooses from at render time.

## Topics

### Creating a color

init(String, bundle: Bundle?)

Creates a color from a color set that you indicate by name.

init(_:)

Creates a constant color with the values specified by the resolved color.

func resolve(in: EnvironmentValues) -> Color.Resolved

Evaluates this color to a resolved color given the current `context`.

### Creating a color from component values

init(hue: Double, saturation: Double, brightness: Double, opacity: Double)

Creates a constant color from hue, saturation, and brightness values.

init(Color.RGBColorSpace, white: Double, opacity: Double)

Creates a constant grayscale color.

init(Color.RGBColorSpace, red: Double, green: Double, blue: Double, opacity: Double)

Creates a constant color from red, green, and blue component values.

enum RGBColorSpace

A profile that specifies how to interpret a color value for display.

### Creating a color from another color

init(uiColor: UIColor)

Creates a color from a UIKit color.

init(nsColor: NSColor)

Creates a color from an AppKit color.

init(cgColor: CGColor)

Creates a color from a Core Graphics color.

### Getting standard colors

static let black: Color

A black color suitable for use in UI elements.

static let blue: Color

A context-dependent blue color suitable for use in UI elements.

static let brown: Color

A context-dependent brown color suitable for use in UI elements.

static let clear: Color

A clear color suitable for use in UI elements.

static let cyan: Color

A context-dependent cyan color suitable for use in UI elements.

static let gray: Color

A context-dependent gray color suitable for use in UI elements.

static let green: Color

A context-dependent green color suitable for use in UI elements.

static let indigo: Color

A context-dependent indigo color suitable for use in UI elements.

static let mint: Color

A context-dependent mint color suitable for use in UI elements.

static let orange: Color

A context-dependent orange color suitable for use in UI elements.

static let pink: Color

A context-dependent pink color suitable for use in UI elements.

static let purple: Color

A context-dependent purple color suitable for use in UI elements.

static let red: Color

A context-dependent red color suitable for use in UI elements.

static let teal: Color

A context-dependent teal color suitable for use in UI elements.

static let white: Color

A white color suitable for use in UI elements.

static let yellow: Color

A context-dependent yellow color suitable for use in UI elements.

### Getting semantic colors

static var accentColor: Color

A color that reflects the accent color of the system or app.

static let primary: Color

The color to use for primary content.

static let secondary: Color

The color to use for secondary content.

### Modifying a color

func opacity(Double) -> Color

Multiplies the opacity of the color by the given amount.

var gradient: AnyGradient

Returns the standard gradient for the color `self`.

### Describing a color

var description: String

A textual representation of the color.

### Comparing colors

static func == (Color, Color) -> Bool

Indicates whether two colors are equal.

func hash(into: inout Hasher)

Hashes the essential components of the color by feeding them into the given hash function.

### Deprecated symbols

var cgColor: CGColor?

A Core Graphics representation of the color, if available.

Deprecated

### Instance Methods

func mix(with: Color, by: Double, in: Gradient.ColorSpace) -> Color

Returns a version of self mixed with `rhs` by the amount specified by `fraction`.

### Default Implementations

ShapeStyle Implementations

Transferable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable
- ShapeStyle
- Transferable
- View

## See Also

### Setting a color

func tint(_:)

Sets the tint color within this view.

