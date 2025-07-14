

- AppKit
- NSColor
-  alphaComponent 

Instance Property

# alphaComponent

The alpha (opacity) component value of the color.

macOS

``` source
var alphaComponent: CGFloat { get }
```

## Discussion

The value of this property is between `0.0` and `1.0`, where `0.0` represents fully transparent and `1.0` represents fully opaque. If the color has no alpha component, the value of this property is `1.0`.

## See Also

### Related Documentation

func getRed(UnsafeMutablePointer&lt;CGFloat>?, green: UnsafeMutablePointer&lt;CGFloat>?, blue: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s RGB component and opacity values in the respective arguments.

func getHue(UnsafeMutablePointer&lt;CGFloat>?, saturation: UnsafeMutablePointer&lt;CGFloat>?, brightness: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s HSB component and opacity values in the respective arguments.

func getCyan(UnsafeMutablePointer&lt;CGFloat>?, magenta: UnsafeMutablePointer&lt;CGFloat>?, yellow: UnsafeMutablePointer&lt;CGFloat>?, black: UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the color object’s CMYK and opacity values.

func getWhite(UnsafeMutablePointer&lt;CGFloat>?, alpha: UnsafeMutablePointer&lt;CGFloat>?)

Returns the grayscale and alpha values of the color.

### Retrieving Individual Components

var whiteComponent: CGFloat

The white component value of the color.

var redComponent: CGFloat

The red component value of the color.

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

