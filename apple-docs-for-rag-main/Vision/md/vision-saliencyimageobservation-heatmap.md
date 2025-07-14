

- Vision
- SaliencyImageObservation
-  heatMap 

Instance Property

# heatMap

A grayscale heat map of important areas across the image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let heatMap: PixelBufferObservation
```

## Discussion

The heat map is a pixel buffer in a one-component floating-point pixel format.

## See Also

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

struct PixelBufferObservation

An object that represents an image that an image-analysis request produces.

let salientObjects: [RectangleObservation]

A collection of objects describing the distinct areas of the saliency heat map.

struct RectangleObservation

An object that represents the four vertices of a detected rectangle.

