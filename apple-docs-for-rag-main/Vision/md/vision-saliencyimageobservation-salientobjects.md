

- Vision
- SaliencyImageObservation
-  salientObjects 

Instance Property

# salientObjects

A collection of objects describing the distinct areas of the saliency heat map.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let salientObjects: [RectangleObservation]
```

## Discussion

The objects in this array don’t follow any specific ordering. It’s up to your app to iterate across the observations and apply desired ordering.

## See Also

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

let heatMap: PixelBufferObservation

A grayscale heat map of important areas across the image.

struct PixelBufferObservation

An object that represents an image that an image-analysis request produces.

struct RectangleObservation

An object that represents the four vertices of a detected rectangle.

