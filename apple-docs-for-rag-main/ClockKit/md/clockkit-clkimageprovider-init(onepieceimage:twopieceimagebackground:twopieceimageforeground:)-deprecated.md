

- ClockKit
- CLKImageProvider
-  init(onePieceImage:twoPieceImageBackground:twoPieceImageForeground:) Deprecated

Initializer

# init(onePieceImage:twoPieceImageBackground:twoPieceImageForeground:)

Creates and returns an image provider with both one-piece and two-piece images.

watchOS 2.0–9.0Deprecated

``` source
convenience init(
    onePieceImage: UIImage,
    twoPieceImageBackground: UIImage?,
    twoPieceImageForeground: UIImage?
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`onePieceImage`  

The one-piece image to use. The image must be a template image, where only the alpha channel is used to define the image contents. This parameter must not be `nil`.

`twoPieceImageBackground`  

The background to use for a two-piece image. The image must be a template image, where only the alpha channel is used to define the image contents. This parameter must not be `nil`.

`twoPieceImageForeground`  

The foreground to use for a two-piece image. The image must be a template image, where only the alpha channel is used to define the image contents. This parameter must not be `nil`.

## Return Value

An image provider with both the one-piece and two-piece images.

## Discussion

Use this method when you want to display a two-piece image in multicolor environments. In monochrome environments, the image provider still displays the one-piece image. After creating the image provider, you can customize the tint color applied to your images by modifying the tintColor property.

## See Also

### Creating an Image Provider

convenience init(onePieceImage: UIImage)

Creates and returns an image provider with the specified one-piece image.

Deprecated

