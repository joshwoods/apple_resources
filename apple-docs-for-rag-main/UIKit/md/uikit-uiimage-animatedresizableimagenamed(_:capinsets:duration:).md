

- UIKit
- UIImage
-  animatedResizableImageNamed(\_:capInsets:duration:) 

Type Method

# animatedResizableImageNamed(\_:capInsets:duration:)

Creates and returns an animated image with end caps.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func animatedResizableImageNamed(
    _ name: String,
    capInsets: UIEdgeInsets,
    duration: TimeInterval
) -> UIImage?
```

## Parameters 

`name`  

The full or partial path to the file (sans suffix).

`capInsets`  

The values to use for the cap insets.

`duration`  

The duration of the animation.

## Return Value

A new image object.

## Discussion

This method loads a series of files by appending a series of numbers to the base file name provided in the `name` parameter. For example, if the `name` parameter had ‘image’ as its contents, this method would attempt to load images from files with the names ‘image0’, ‘image1’ and so on all the way up to ‘image1024’. All images included in the animated image should share the same size and scale.

Each frame in the animation follows the rules for resizable images created by the resizableImage(withCapInsets:) method.

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

class func animatedResizableImageNamed(String, capInsets: UIEdgeInsets, resizingMode: UIImage.ResizingMode, duration: TimeInterval) -> UIImage?

Creates and returns an animated image with end caps and a specific resizing mode.

