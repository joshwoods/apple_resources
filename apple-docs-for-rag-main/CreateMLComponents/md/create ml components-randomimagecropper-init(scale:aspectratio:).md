

- Create ML Components
- RandomImageCropper
-  init(scale:aspectRatio:) 

Initializer

# init(scale:aspectRatio:)

Creates an augmentation that crops an input image at a random location with a scale that indicates the lower and upper bounds to randomly scale the height and width of the image. The range must be between 0 and 1.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
init(
    scale: ClosedRange,
    aspectRatio: Double? = nil
)
```

## Parameters 

`scale`  

A range of scales.

`aspectRatio`  

A size that specifies the ratio of width to height to use for the cropping rectangle.

## See Also

### Creating an image cropper

init(targetSize: CGSize)

Creates an augmentation that crops an input image at a random location to the specified target size.

init(targetWidth: Double, targetHeight: Double)

Creates an augmentation that crops an input image at a random location to the specified target width and height.

