

- AppKit
- NSGradient
-  colorSpace 

Instance Property

# colorSpace

The color space of the colors associated with the gradient.

macOS 10.5+

``` source
var colorSpace: NSColorSpace { get }
```

## Discussion

When the receiver is initialized, colors that do not conform to the receiver’s color space are converted automatically.

## See Also

### Getting Gradient Properties

var numberOfColorStops: Int

The number of color stops associated with the gradient.

func getColor(AutoreleasingUnsafeMutablePointer&lt;NSColor>?, location: UnsafeMutablePointer&lt;CGFloat>?, at: Int)

Returns information about the color stop at the specified index in the receiver’s color array.

func interpolatedColor(atLocation: CGFloat) -> NSColor

Returns the color of the rendered gradient at the specified relative location.

