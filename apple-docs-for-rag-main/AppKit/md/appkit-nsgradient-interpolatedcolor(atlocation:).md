

- AppKit
- NSGradient
-  interpolatedColor(atLocation:) 

Instance Method

# interpolatedColor(atLocation:)

Returns the color of the rendered gradient at the specified relative location.

macOS 10.5+

``` source
func interpolatedColor(atLocation location: CGFloat) -> NSColor
```

## Parameters 

`location`  

The location value for the color you want. This value must be between 0.0 and 1.0. This value need not correspond to the location of one of the color objects used to create the gradient.

## Discussion

This method does not simply return the color values used to initialize the receiver. Instead, it computes the value that would be drawn at the specified location.

The start color of the gradient is always located at 0.0 and the end color is always at 1.0.

## See Also

### Getting Gradient Properties

var colorSpace: NSColorSpace

The color space of the colors associated with the gradient.

var numberOfColorStops: Int

The number of color stops associated with the gradient.

func getColor(AutoreleasingUnsafeMutablePointer&lt;NSColor>?, location: UnsafeMutablePointer&lt;CGFloat>?, at: Int)

Returns information about the color stop at the specified index in the receiver’s color array.

