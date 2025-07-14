

- Core Image
- CIFilter
- Stylizing Filters
- CILineOverlay
-  edgeIntensity 

Instance Property

# edgeIntensity

The accentuation factor of the Sobel gradient information when tracing the edges of the image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var edgeIntensity: Float { get set }
```

**Required**

## Discussion

Higher values find more edges, although typically, you’d use a low value (such as 1.0).

