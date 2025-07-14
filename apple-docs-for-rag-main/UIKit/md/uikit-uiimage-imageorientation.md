

- UIKit
- UIImage
-  imageOrientation 

Instance Property

# imageOrientation

The orientation of the receiver’s image.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var imageOrientation: UIImage.Orientation { get }
```

## Discussion

Image orientation affects the way the image data is displayed when drawn. By default, images are displayed in the “up” orientation. If the image has associated metadata (such as EXIF information), however, this property contains the orientation indicated by that metadata. For a list of possible values for this property, see UIImage.Orientation.

## See Also

### Accessing image attributes

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

var alignmentRectInsets: UIEdgeInsets

The alignment metadata for positioning the image during layout.

var isSymbolImage: Bool

A Boolean value that indicates whether the image is a symbol.

