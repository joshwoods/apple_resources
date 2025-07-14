

- ClockKit
- CLKFullColorImageProvider
-  init(fullColorImage:) Deprecated

Initializer

# init(fullColorImage:)

Creates an image provider with the specified full-color image.

watchOS 5.0–9.0Deprecated

``` source
convenience init(fullColorImage image: UIImage)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`image`  

The image to display.

## Return Value

A full-color image provider.

## Discussion

For information about the image sizes and masks, see Apple Watch Human Interface Guidelines.

## See Also

### Creating an Image Provider

convenience init(fullColorImage: UIImage, tintedImageProvider: CLKImageProvider?)

Creates an image provider that produces full-color and tinted images.

Deprecated

