

- UIKit
- UIScreen
-  nativeBounds 

Instance Property

# nativeBounds

The bounding rectangle of the physical screen, measured in pixels.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS

``` source
@MainActor
var nativeBounds: CGRect { get }
```

## Discussion

This rectangle is based on the device in a portrait-up orientation. This value does not change as the device rotates.

## See Also

### Getting the size and scale

var bounds: CGRect

The bounding rectangle of the screen, measured in points.

var nativeScale: CGFloat

The native scale factor for the physical screen.

var scale: CGFloat

The natural scale factor associated with the screen.

