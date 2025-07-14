

- UIKit
- UIImage
- UIImage.Orientation
-  UIImage.Orientation.up 

Case

# UIImage.Orientation.up

The original pixel data matches the image’s intended display orientation.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
case up
```

## Discussion

If an image is encoded with this orientation, then displayed by software unaware of orientation metadata, the image appears correctly “right side up”. That is, this orientation is an identity value.

## See Also

### Related Documentation

case up

The encoded image data matches the image’s intended display orientation.

### Image orientations

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

