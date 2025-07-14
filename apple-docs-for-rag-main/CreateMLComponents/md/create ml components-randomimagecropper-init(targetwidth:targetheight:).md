

- Create ML Components
- RandomImageCropper
-  init(targetWidth:targetHeight:) 

Initializer

# init(targetWidth:targetHeight:)

Creates an augmentation that crops an input image at a random location to the specified target width and height.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
init(
    targetWidth: Double,
    targetHeight: Double
)
```

## Parameters 

`targetWidth`  

The target width of the cropping rectangle. Must be positive.

`targetHeight`  

The target height of the cropping rectangle. Must be positive.

## See Also

### Creating an image cropper

init(scale: ClosedRange&lt;Double>, aspectRatio: Double?)

Creates an augmentation that crops an input image at a random location with a scale that indicates the lower and upper bounds to randomly scale the height and width of the image. The range must be between 0 and 1.

init(targetSize: CGSize)

Creates an augmentation that crops an input image at a random location to the specified target size.

