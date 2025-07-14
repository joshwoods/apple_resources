

- Core Image
- CIColor
-  stringRepresentation 

Instance Property

# stringRepresentation

A formatted string that specifies the components of the color.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
var stringRepresentation: String { get }
```

## Discussion

The string representation always has four components—red, green, blue, and alpha. The default value for the alpha component is `1.0`. For example, this string:

`@"0.5 0.7 0.3 1.0"`

indicates an RGB color whose components are 50% red, 70% green, 30% blue, and 100% opaque (alpha value of `1.0`).

## See Also

### Getting Color Components

var colorSpace: CGColorSpace

The Quartz 2D color space associated with the color.

var components: UnsafePointer&lt;CGFloat>

The color components of the color.

var numberOfComponents: Int

Returns the number of color components in the color.

var red: CGFloat

The unpremultiplied red component of the color.

var green: CGFloat

The unpremultiplied green component of the color.

var blue: CGFloat

The unpremultiplied blue component of the color.

var alpha: CGFloat

The alpha value of the color.

