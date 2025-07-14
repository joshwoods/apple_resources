

- MapKit
- MKGradientPolylineRenderer
-  colors 

Instance Property

# colors

An array that represents the gradient’s color transition points.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
var colors: [UIColor] { get }
```

**macOS**

``` source
var colors: [NSColor] { get }
```

## See Also

### Accessing the gradient colors

func setColors([UIColor], locations: [CGFloat])

Sets the iOS colors and corresponding unit distance values to create gradients.

func setColors([NSColor], locations: [CGFloat])

Sets the macOS colors and corresponding unit distance values to create gradients.

var locations: [CGFloat]

An array of location indexes that correspond to their respective colors.

