

- ClockKit
- CLKFullColorImageProvider
-  init(fullColorImage:tintedImageProvider:) Deprecated

Initializer

# init(fullColorImage:tintedImageProvider:)

Creates an image provider that produces full-color and tinted images.

watchOS 6.0–9.0Deprecated

``` source
convenience init(
    fullColorImage image: UIImage,
    tintedImageProvider: CLKImageProvider?
)
```

## Parameters 

`image`  

The image to display for full-color complications.

`tintedImageProvider`  

An image provider that produces images for tinted complications.

## Return Value

An image provider that produces full-color and tinted images. For more information about tinted images, see tintedImageProvider.

## Discussion

For information about the image sizes and masks used by the different complication families, see Complication Images.

## See Also

### Creating an Image Provider

convenience init(fullColorImage: UIImage)

Creates an image provider with the specified full-color image.

Deprecated

