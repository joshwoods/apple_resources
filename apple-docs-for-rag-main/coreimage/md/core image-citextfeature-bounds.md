

- Core Image
- CITextFeature
-  bounds 

Instance Property

# bounds

A rectangle indicating the position and extent of the feature in image coordinates.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var bounds: CGRect { get }
```

## Discussion

This property identifies the rectangular region *of the image* containing the detected text region, not necessarily the shape of the region. A detected feature is rectangular in space, but may appear in perspective in the image. Use the properties listed in Identifying the Corners of a Detected Text Region to find the corners of the rectangle as it appears in perspective.

## See Also

### Related Documentation

Core Image Programming Guide

