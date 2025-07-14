

- Core ML
- MLTensor
- MLTensor.ResizeMethod
-  MLTensor.ResizeMethod.bilinear(alignCorners:) 

Case

# MLTensor.ResizeMethod.bilinear(alignCorners:)

The bilinear interpolation mode where values are computed using bilinear interpolation of 4 neighboring pixels.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
case bilinear(alignCorners: Bool = false)
```

## Discussion

`alignCorners` is a Boolean indicating whether to align the corners of the upscaling grid to the centre of the scaling dimensions rather than the edges.

