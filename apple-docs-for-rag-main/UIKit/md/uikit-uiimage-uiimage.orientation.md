

- UIKit
- UIImage
-  UIImage.Orientation 

Enumeration

# UIImage.Orientation

Constants that specify the intended display orientation for an image.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
enum Orientation
```

## Overview

Orientation values are commonly found in image metadata, and specifying image orientation correctly can be important both for displaying the image and for certain kinds of image processing.

The UIImage class automatically handles the transform necessary to present an image in the correct display orientation according to its orientation metadata, so an image object’s imageOrientation property simply indicates which transform was applied.

For example, an iOS device camera always encodes pixel data in the camera sensor’s native landscape orientation, along with metadata indicating the camera orientation. When UIImage loads a photo shot in portrait orientation, it automatically applies a 90° rotation before displaying the image data, and the image’s imageOrientation value of UIImage.Orientation.right indicates that this rotation has been applied.

Note

Some frameworks describe image orientation using the CGImagePropertyOrientation type (or the raw TIFF/Exif numeric values that type defines symbols for). However, the underlying numeric values of that type are incompatible with UIImage.Orientation. For conversion help, see the CGImagePropertyOrientation overview.

## Topics

### Image orientations

case up

The original pixel data matches the image’s intended display orientation.

case down

The image has been rotated 180° from the orientation of its original pixel data.

case left

The image has been rotated 90° counterclockwise from the orientation of its original pixel data.

case right

The image has been rotated 90° clockwise from the orientation of its original pixel data.

case upMirrored

The image has been horizontally flipped from the orientation of its original pixel data.

case downMirrored

The image has been vertically flipped from the orientation of its original pixel data.

case leftMirrored

The image has been rotated 90° clockwise and flipped horizontally from the orientation of its original pixel data.

case rightMirrored

The image has been rotated 90° counterclockwise and flipped horizontally from the orientation of its original pixel data.

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

### Related Documentation

@frozen enum CGImagePropertyOrientation

A value describing the intended display orientation for an image.

### Accessing image attributes

var imageOrientation: UIImage.Orientation

The orientation of the receiver’s image.

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

