

- UIKit
- UIScreen
-  bounds 

Instance Property

# bounds

The bounding rectangle of the screen, measured in points.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOS

``` source
@MainActor
var bounds: CGRect { get }
```

## Discussion

This rectangle is specified in the current coordinate space, which takes into account any interface rotations in effect for the device. Therefore, the value of this property may change when the device rotates between portrait and landscape orientations.

## See Also

### Getting the size and scale

var nativeBounds: CGRect

The bounding rectangle of the physical screen, measured in pixels.

var nativeScale: CGFloat

The native scale factor for the physical screen.

var scale: CGFloat

The natural scale factor associated with the screen.

