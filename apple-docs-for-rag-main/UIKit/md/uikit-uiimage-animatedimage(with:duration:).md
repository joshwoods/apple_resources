

- UIKit
- UIImage
-  animatedImage(with:duration:) 

Type Method

# animatedImage(with:duration:)

Creates and returns an animated image from an existing set of images.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func animatedImage(
    with images: [UIImage],
    duration: TimeInterval
) -> UIImage?
```

## Parameters 

`images`  

An array of UIImage objects.

`duration`  

The duration of the animation.

## Return Value

A new image object.

## Discussion

All images included in the animated image should share the same size and scale.

## See Also

### Creating animated images

class func animatedImageNamed(String, duration: TimeInterval) -> UIImage?

Creates and returns an animated image.

class func animatedResizableImageNamed(String, capInsets: UIEdgeInsets, duration: TimeInterval) -> UIImage?

Creates and returns an animated image with end caps.

class func animatedResizableImageNamed(String, capInsets: UIEdgeInsets, resizingMode: UIImage.ResizingMode, duration: TimeInterval) -> UIImage?

Creates and returns an animated image with end caps and a specific resizing mode.

