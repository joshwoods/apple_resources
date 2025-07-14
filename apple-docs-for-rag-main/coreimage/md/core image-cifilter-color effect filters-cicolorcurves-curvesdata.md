

- Core Image
- CIFilter
- Color Effect Filters
- CIColorCurves
-  curvesData 

Instance Property

# curvesData

Color values that determine the color curves transform.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var curvesData: Data { get set }
```

**Required**

## Discussion

Create the curves data as an NSData object containing a sequence of single-precision RGB values. These values represent a lookup table that’s applied to the input image.

Core Image unpremultiplies the image before applying the effect, and premultiplies the result after applying the effect.

