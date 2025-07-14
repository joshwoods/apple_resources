

- AppKit
- NSColor
-  redComponent 

Instance Property

# redComponent

The red component value of the color.

macOS

``` source
var redComponent: CGFloat { get }
```

## Discussion

Access this property only for colors in the calibratedRGB or deviceRGB color spaces. Accessing it for other color types raises an exception.

## See Also

### Related Documentation

func getRed(UnsafeMutablePointer&lt;CGFloat>?, green: UnsafeMutablePointer&lt;CGFloat>?, blue: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s RGB component and opacity values in the respective arguments.

### Retrieving Individual Components

var alphaComponent: CGFloat

The alpha (opacity) component value of the color.

var whiteComponent: CGFloat

The white component value of the color.

var greenComponent: CGFloat

The green component value of the color.

var blueComponent: CGFloat

The blue component value of the color.

var cyanComponent: CGFloat

The cyan component value of the color.

var magentaComponent: CGFloat

The magenta component value of the color.

var yellowComponent: CGFloat

The yellow component value of the color.

var blackComponent: CGFloat

The black component value of the color.

var hueComponent: CGFloat

The hue component value of the color.

var saturationComponent: CGFloat

The saturation component value of the color.

var brightnessComponent: CGFloat

The brightness component value of the color.

var catalogNameComponent: NSColorList.Name

The catalog containing the color’s name.

var localizedCatalogNameComponent: String

The localized version of the catalog name containing the color.

var colorNameComponent: NSColor.Name

The name of the color.

var localizedColorNameComponent: String

The localized version of the color name.

