

- AppKit
- NSColor
- NSColor.ColorType
-  NSColor.ColorType.componentBased 

Case

# NSColor.ColorType.componentBased

Colors that include floating-point color components and a color space.

macOS

``` source
case componentBased
```

## Discussion

Examples of this type are RGB, CMYK, and HSB colors. Before acessing components that are specific to one colorspace, such as the redComponent of an RGB color, call usingColorSpace(_:).

## See Also

### Color Types

case pattern

Colors that include an image to be used as a pattern.

case catalog

Colors that are retrieved from an asset catalog.

