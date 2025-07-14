

- Create ML Components
- RandomImageCropper
-  applied(to:generator:eventHandler:) 

Instance Method

# applied(to:generator:eventHandler:)

Randomly crops an image at a random location of a given size.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func applied(
    to image: CIImage,
    generator: inout some RandomNumberGenerator,
    eventHandler: EventHandler? = nil
) async throws -> CIImage
```

## Parameters 

`image`  

The input image.

`generator`  

A random number generator.

`eventHandler`  

An event handler.

## Return Value

The cropped image.

