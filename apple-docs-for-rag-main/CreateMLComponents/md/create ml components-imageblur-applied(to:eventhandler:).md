

- Create ML Components
- ImageBlur
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Blurs an image using a disc-shaped convolution kernel.

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

The blurry image.

