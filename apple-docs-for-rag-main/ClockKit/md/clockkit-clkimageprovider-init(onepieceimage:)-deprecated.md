

- ClockKit
- CLKImageProvider
-  init(onePieceImage:) Deprecated

Initializer

# init(onePieceImage:)

Creates and returns an image provider with the specified one-piece image.

watchOS 2.0–9.0Deprecated

``` source
convenience init(onePieceImage: UIImage)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`onePieceImage`  

The image to display. The image must be a template image, where only the alpha channel is used to define the image contents. This parameter must not be `nil`.

## Return Value

An image provider with only the one-piece image.

## Discussion

Use this method to create an image provider with only a one-piece image. The resulting image provider displays the one-piece image in all contexts. After creating the image provider, you can customize the tint color applied to your image by modifying the tintColor property.

## See Also

### Creating an Image Provider

convenience init(onePieceImage: UIImage, twoPieceImageBackground: UIImage?, twoPieceImageForeground: UIImage?)

Creates and returns an image provider with both one-piece and two-piece images.

Deprecated

