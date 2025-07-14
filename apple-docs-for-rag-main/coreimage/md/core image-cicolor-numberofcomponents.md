

- Core Image
- CIColor
-  numberOfComponents 

Instance Property

# numberOfComponents

Returns the number of color components in the color.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
var numberOfComponents: Int { get }
```

## Discussion

This number includes the alpha component if the color contains one.

## See Also

### Getting Color Components

var colorSpace: CGColorSpace

The Quartz 2D color space associated with the color.

var components: UnsafePointer&lt;CGFloat>

The color components of the color.

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

