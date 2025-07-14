

- Create ML Components
- ImageScaler
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Perform the image scaler operation on the input pixelBuffer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func applied(
    to image: CIImage,
    eventHandler: EventHandler? = nil
) throws -> CIImage
```

## Parameters 

`image`  

An image.

`eventHandler`  

An event handler.

## Return Value

The scaled pixel buffer.

