

- Image I/O
- CGImagePropertyOrientation
-  CGImagePropertyOrientation.rightMirrored 

Case

# CGImagePropertyOrientation.rightMirrored

The encoded image data is horizontally flipped and rotated 90° clockwise from the image’s intended display orientation.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case rightMirrored
```

## Discussion

The (x,y) pixel coordinates of the origin point (0,0) represent the bottom row and rightmost column, respectively. Pixel (x,y) positions increase bottom-to-top, right-to-left.

If an image is encoded with this orientation, then displayed by software unaware of orientation metadata, the image appears to be horizontally mirrored, then rotated 90° clockwise. (That is, to present the image in its intended orientation, you can rotate 90° counter-clockwise, then flip horizontally.)

## See Also

### Image Orientations

case up

The encoded image data matches the image’s intended display orientation.

case upMirrored

The encoded image data is horizontally flipped from the image’s intended display orientation.

case down

The encoded image data is rotated 180° from the image’s intended display orientation.

case downMirrored

The encoded image data is vertically flipped from the image’s intended display orientation.

case leftMirrored

The encoded image data is horizontally flipped and rotated 90° counter-clockwise from the image’s intended display orientation.

case right

The encoded image data is rotated 90° clockwise from the image’s intended display orientation.

case left

The encoded image data is rotated 90° clockwise from the image’s intended display orientation.

