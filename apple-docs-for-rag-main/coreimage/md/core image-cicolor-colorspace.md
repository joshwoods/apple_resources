

- Core Image
- CIColor
-  colorSpace 

Instance Property

# colorSpace

The Quartz 2D color space associated with the color.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
var colorSpace: CGColorSpace { get }
```

## See Also

### Getting Color Components

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

var stringRepresentation: String

A formatted string that specifies the components of the color.

