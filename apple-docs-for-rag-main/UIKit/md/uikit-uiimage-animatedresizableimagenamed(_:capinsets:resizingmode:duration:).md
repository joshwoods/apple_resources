

- UIKit
- UIImage
-  animatedResizableImageNamed(\_:capInsets:resizingMode:duration:) 

Type Method

# animatedResizableImageNamed(\_:capInsets:resizingMode:duration:)

Creates and returns an animated image with end caps and a specific resizing mode.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func animatedResizableImageNamed(
    _ name: String,
    capInsets: UIEdgeInsets,
    resizingMode: UIImage.ResizingMode,
    duration: TimeInterval
) -> UIImage?
```

## Parameters 

`name`  

The full or partial path to the file (sans suffix).

`capInsets`  

The values to use for the cap insets.

`resizingMode`  

The mode with which the interior of the image is resized.

`duration`  

The duration of the animation.

## Return Value

A new animated image object with the specified cap insets and resizing mode.

## Discussion

This method is exactly the same as its counterpart animatedResizableImageNamed(_:capInsets:duration:) except that the resizing mode of the new image object can be explicitly declared. Since the resizing mode of an image is UIImage.ResizingMode.tile by default, this method should only be used in place of its counterpart to create an animated image that needs to be resized with the UIImage.ResizingMode.stretch resizing mode.

## See Also

### Related Documentation

func resizableImage(withCapInsets: UIEdgeInsets) -> UIImage

Returns a new version of the image with the specified cap insets.

func resizableImage(withCapInsets: UIEdgeInsets, resizingMode: UIImage.ResizingMode) -> UIImage

Returns a new version of the image with the specified cap insets and options.

### Creating animated images

class func animatedImageNamed(String, duration: TimeInterval) -> UIImage?

Creates and returns an animated image.

class func animatedImage(with: [UIImage], duration: TimeInterval) -> UIImage?

Creates and returns an animated image from an existing set of images.

class func animatedResizableImageNamed(String, capInsets: UIEdgeInsets, duration: TimeInterval) -> UIImage?

Creates and returns an animated image with end caps.

