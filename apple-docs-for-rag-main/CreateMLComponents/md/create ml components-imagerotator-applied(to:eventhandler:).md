

- Create ML Components
- ImageRotator
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Rotates the image and then scales and crops the rotated image to fit the extent of the input image.

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

The rotated image.

