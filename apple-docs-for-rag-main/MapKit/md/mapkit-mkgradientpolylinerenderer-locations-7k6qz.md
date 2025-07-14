

- MapKit
- MKGradientPolylineRenderer
-  locations 

Instance Property

# locations

An array of location indexes that correspond to their respective colors.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOS

``` source
var locations: [CGFloat] { get }
```

## See Also

### Accessing the gradient colors

func setColors([UIColor], locations: [CGFloat])

Sets the iOS colors and corresponding unit distance values to create gradients.

func setColors([NSColor], locations: [CGFloat])

Sets the macOS colors and corresponding unit distance values to create gradients.

var colors: [UIColor]

An array that represents the gradient’s color transition points.

