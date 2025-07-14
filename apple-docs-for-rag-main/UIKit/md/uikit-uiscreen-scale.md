

- UIKit
- UIScreen
-  scale 

Instance Property

# scale

The natural scale factor associated with the screen.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOS

``` source
@MainActor
var scale: CGFloat { get }
```

## Discussion

This value reflects the scale factor needed to convert from the default logical coordinate space into the device coordinate space of this screen. The default logical coordinate space is measured using points. For Retina displays, the scale factor may be `3.0` or `2.0` and one point can represented by nine or four pixels, respectively. For standard-resolution displays, the scale factor is `1.0` and one point equals one pixel.

## See Also

### Getting the size and scale

var bounds: CGRect

The bounding rectangle of the screen, measured in points.

var nativeBounds: CGRect

The bounding rectangle of the physical screen, measured in pixels.

var nativeScale: CGFloat

The native scale factor for the physical screen.

