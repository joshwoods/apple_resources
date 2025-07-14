

- UIKit
- UIImage
- UIImage.Orientation
-  UIImage.Orientation.left 

Case

# UIImage.Orientation.left

The image has been rotated 90° counterclockwise from the orientation of its original pixel data.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
case left
```

## Discussion

If an image is encoded with this orientation, then displayed by software unaware of orientation metadata, the image appears to be rotated 90° clockwise. (That is, to present the image in its intended orientation, you must rotate 90° counter-clockwise.)

## See Also

### Related Documentation

case left

The encoded image data is rotated 90° clockwise from the image’s intended display orientation.

### Image orientations

case up

The original pixel data matches the image’s intended display orientation.

case down

The image has been rotated 180° from the orientation of its original pixel data.

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

