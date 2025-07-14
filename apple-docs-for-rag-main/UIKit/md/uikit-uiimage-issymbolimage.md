

- UIKit
- UIImage
-  isSymbolImage 

Instance Property

# isSymbolImage

A Boolean value that indicates whether the image is a symbol.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var isSymbolImage: Bool { get }
```

## Discussion

Symbol images are vector-based images that you use for your app’s iconography. The value of this property is true if the image is either a system-provided symbol image or a custom symbol image that you supplied in your asset catalog. The value is false for all other image types.

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

var alignmentRectInsets: UIEdgeInsets

The alignment metadata for positioning the image during layout.

