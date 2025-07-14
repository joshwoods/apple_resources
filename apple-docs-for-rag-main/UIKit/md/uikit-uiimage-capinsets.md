

- UIKit
- UIImage
-  capInsets 

Instance Property

# capInsets

The end-cap insets.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var capInsets: UIEdgeInsets { get }
```

## Discussion

End caps specify the portion of an image that should not be resized when an image is stretched. This technique is used to implement buttons and other resizable image-based interface elements. When a button with end caps is resized, the resizing occurs only in the middle of the button, in the region between the end caps. The end caps themselves keep their original size and appearance.

This property specifies the sizes of all four end caps. The middle (stretchable) portion consists of all the pixels that are not included in the end caps. These pixels are tiled, left-to-right, top-to-bottom to fill the remaining space.

On a non-resizable image, this property is set to `UIEdgeInsetsZero`; the image does not use end caps and the entire image is subject to stretching. To create a new image with a nonzero value for this property, use the resizableImage(withCapInsets:) method. If your application specifies `UIEdgeInsetsZero` as the `capInsets` parameter, the entire image is tiled.

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

var alignmentRectInsets: UIEdgeInsets

The alignment metadata for positioning the image during layout.

var isSymbolImage: Bool

A Boolean value that indicates whether the image is a symbol.

