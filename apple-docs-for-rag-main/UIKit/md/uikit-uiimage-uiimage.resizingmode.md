

- UIKit
- UIImage
-  UIImage.ResizingMode 

Enumeration

# UIImage.ResizingMode

Constants that specify the possible resizing modes for an image.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
enum ResizingMode
```

## Topics

### Constants

case tile

The image is tiled when it is resized. In other words, the interior region of the original image will be repeated to fill in the interior region of the newly resized image.

case stretch

The image is stretched when it is resized. In other words, the interior region of the original image will be scaled to fill in the interior region of the newly resized imaged.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var duration: TimeInterval

The time interval for displaying an animated image.

var capInsets: UIEdgeInsets

The end-cap insets.

var alignmentRectInsets: UIEdgeInsets

The alignment metadata for positioning the image during layout.

var isSymbolImage: Bool

A Boolean value that indicates whether the image is a symbol.

