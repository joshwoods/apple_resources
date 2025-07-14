

- Image I/O
- CGImagePropertyOrientation
-  CGImagePropertyOrientation.down 

Case

# CGImagePropertyOrientation.down

The encoded image data is rotated 180° from the image’s intended display orientation.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case down
```

## Discussion

The (x,y) pixel coordinates of the origin point (0,0) represent the rightmost column and bottom row, respectively. Pixel (x,y) positions increase right-to-left, bottom-to-top.

If an image is encoded with this orientation, then displayed by software unaware of orientation metadata, the image appears rotated 180°.

## See Also

### Image Orientations

case up

The encoded image data matches the image’s intended display orientation.

case upMirrored

The encoded image data is horizontally flipped from the image’s intended display orientation.

case downMirrored

The encoded image data is vertically flipped from the image’s intended display orientation.

case leftMirrored

The encoded image data is horizontally flipped and rotated 90° counter-clockwise from the image’s intended display orientation.

case right

The encoded image data is rotated 90° clockwise from the image’s intended display orientation.

case rightMirrored

The encoded image data is horizontally flipped and rotated 90° clockwise from the image’s intended display orientation.

case left

The encoded image data is rotated 90° clockwise from the image’s intended display orientation.

