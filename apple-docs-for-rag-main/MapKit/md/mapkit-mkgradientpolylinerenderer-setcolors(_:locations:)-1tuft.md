

- MapKit
- MKGradientPolylineRenderer
-  setColors(\_:locations:) 

Instance Method

# setColors(\_:locations:)

Sets the macOS colors and corresponding unit distance values to create gradients.

iOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+

``` source
func setColors(
    _ colors: [NSColor],
    locations: [CGFloat]
)
```

## Parameters 

`colors`  

An array of colors making up the transition points of the gradient.

`locations`  

An array of unit distance values that correspond to the provided colors.

## Discussion

The unit distance value of `0` represents the start of the polyline, and `1` represents the end of the polyline. A gradient may have any number of steps along the length of the polyline.

To determine a location along the polyline, use location(atPointIndex:), or retrieve a set of locations using locations.

## See Also

### Accessing the gradient colors

func setColors([UIColor], locations: [CGFloat])

Sets the iOS colors and corresponding unit distance values to create gradients.

var colors: [UIColor]

An array that represents the gradient’s color transition points.

var locations: [CGFloat]

An array of location indexes that correspond to their respective colors.

