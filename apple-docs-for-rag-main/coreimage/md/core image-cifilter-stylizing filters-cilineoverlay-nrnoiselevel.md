

- Core Image
- CIFilter
- Stylizing Filters
- CILineOverlay
-  nrNoiseLevel 

Instance Property

# nrNoiseLevel

The noise level of the image, used with camera data, that's removed before tracing the edges of the image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var nrNoiseLevel: Float { get set }
```

**Required**

## Discussion

Increasing the noise level helps to clean up the traced edges of the image.

