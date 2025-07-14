

- UIKit
- UIImage
-  alignmentRectInsets 

Instance Property

# alignmentRectInsets

The alignment metadata for positioning the image during layout.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var alignmentRectInsets: UIEdgeInsets { get }
```

## Discussion

You can use the inset values as a hint for specifying the image contents more precisely. For example, if you have a 20 x 20 pixel icon that includes a glow effect, you might set the insets to {{2, 2}, {16, 16}} to indicate the position of the underlying icon without the glow effect.

Objects that incorporate images can use these insets to place the image properly within their content.

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

var duration: TimeInterval

The time interval for displaying an animated image.

var capInsets: UIEdgeInsets

The end-cap insets.

var isSymbolImage: Bool

A Boolean value that indicates whether the image is a symbol.

