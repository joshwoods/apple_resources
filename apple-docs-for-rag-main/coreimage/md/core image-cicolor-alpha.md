

- Core Image
- CIColor
-  alpha 

Instance Property

# alpha

The alpha value of the color.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
var alpha: CGFloat { get }
```

## Discussion

A color created without an explicit alpha value has an alpha of `1.0` by default.

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

var stringRepresentation: String

A formatted string that specifies the components of the color.

