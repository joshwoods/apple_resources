

- Create ML Components
- ImageColorTransformer
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs the image color transformation operation on the input image.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func applied(
    to image: CIImage,
    eventHandler: EventHandler? = nil
) -> CIImage
```

## Parameters 

`image`  

An image.

`eventHandler`  

An event handler.

## Return Value

The color transformed image.

