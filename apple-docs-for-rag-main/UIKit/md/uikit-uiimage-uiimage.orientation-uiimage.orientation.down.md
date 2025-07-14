

- UIKit
- UIImage
- UIImage.Orientation
-  UIImage.Orientation.down 

Case

# UIImage.Orientation.down

The image has been rotated 180° from the orientation of its original pixel data.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
case down
```

## Discussion

If an image is encoded with this orientation, then displayed by software unaware of orientation metadata, the image appears rotated 180°.

## See Also

### Related Documentation

case down

The encoded image data is rotated 180° from the image’s intended display orientation.

### Image orientations

case up

The original pixel data matches the image’s intended display orientation.

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

