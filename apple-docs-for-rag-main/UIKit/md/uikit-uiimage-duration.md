

- UIKit
- UIImage
-  duration 

Instance Property

# duration

The time interval for displaying an animated image.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var duration: TimeInterval { get }
```

## Discussion

For a non-animated image, the value of this property is `0.0`.

## See Also

### Accessing image attributes

var imageOrientation: UIImage.Orientation

The orientation of the receiver’s image.

enum Orientation

Constants that specify the intended display orientation for an image.

var flipsForRightToLeftLayoutDirection: Bool

A Boolean value that indicates whether the image flips in a right-to-left layout.

var resizingMode: UIImage.ResizingMode

The resizing mode of the image.

enum ResizingMode

Constants that specify the possible resizing modes for an image.

var capInsets: UIEdgeInsets

The end-cap insets.

var alignmentRectInsets: UIEdgeInsets

The alignment metadata for positioning the image during layout.

var isSymbolImage: Bool

A Boolean value that indicates whether the image is a symbol.

