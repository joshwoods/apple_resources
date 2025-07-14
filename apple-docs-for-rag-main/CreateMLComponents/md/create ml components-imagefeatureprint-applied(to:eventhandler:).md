

- Create ML Components
- ImageFeaturePrint
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Extracts image features from an image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func applied(
    to image: CIImage,
    eventHandler: EventHandler? = nil
) async throws -> MLShapedArray
```

## Parameters 

`image`  

An image.

`eventHandler`  

An event handler.

## Return Value

A shaped array containing the extracted features of the image.

