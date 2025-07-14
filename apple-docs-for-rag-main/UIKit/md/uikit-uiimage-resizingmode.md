

- UIKit
- UIImage
-  resizingMode 

Instance Property

# resizingMode

The resizing mode of the image.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var resizingMode: UIImage.ResizingMode { get }
```

## Discussion

The default value for this property is UIImage.ResizingMode.tile. However, UIImage will implement the resizing mode the fastest way possible while still retaining the desired visual appearance. This means that if the region to be resized is a 1-pixel region and this property is set to UIImage.ResizingMode.tile, the region will be stretched instead because the two are virtually indistinguishable for a region of that size and stretching is dramatically faster than tiling. To set the value of this property, you need to call either animatedResizableImageNamed(_:capInsets:resizingMode:duration:) or resizableImage(withCapInsets:resizingMode:) and specify the resizing mode using the `resizingMode` parameter. For a list of possible values for this property, see UIImage.ResizingMode.

## See Also

### Accessing image attributes

var imageOrientation: UIImage.Orientation

The orientation of the receiver’s image.

enum Orientation

Constants that specify the intended display orientation for an image.

var flipsForRightToLeftLayoutDirection: Bool

A Boolean value that indicates whether the image flips in a right-to-left layout.

enum ResizingMode

Constants that specify the possible resizing modes for an image.

var duration: TimeInterval

The time interval for displaying an animated image.

var capInsets: UIEdgeInsets

The end-cap insets.

var alignmentRectInsets: UIEdgeInsets

The alignment metadata for positioning the image during layout.

var isSymbolImage: Bool

A Boolean value that indicates whether the image is a symbol.

