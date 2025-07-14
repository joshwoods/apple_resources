

- AppKit
- NSGradient
-  numberOfColorStops 

Instance Property

# numberOfColorStops

The number of color stops associated with the gradient.

macOS 10.5+

``` source
var numberOfColorStops: Int { get }
```

## Discussion

Gradients must have at least two color stops: one defining the location of the start color and one defining the location of the end color. Gradients may have additional color stops located at different transition points in between the start and end stops.

## See Also

### Getting Gradient Properties

var colorSpace: NSColorSpace

The color space of the colors associated with the gradient.

func getColor(AutoreleasingUnsafeMutablePointer&lt;NSColor>?, location: UnsafeMutablePointer&lt;CGFloat>?, at: Int)

Returns information about the color stop at the specified index in the receiver’s color array.

func interpolatedColor(atLocation: CGFloat) -> NSColor

Returns the color of the rendered gradient at the specified relative location.

