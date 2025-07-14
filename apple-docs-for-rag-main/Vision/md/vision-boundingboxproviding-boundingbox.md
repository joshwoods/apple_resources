

- Vision
- BoundingBoxProviding
-  boundingBox 

Instance Property

# boundingBox

The bounding box of the object.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var boundingBox: NormalizedRect { get }
```

**Required** Default implementation provided.

## Discussion

The coordinate system is normalized to the dimensions of the processed image, with the origin at the lower-left corner of the image.

## Default Implementations

### BoundingBoxProviding Implementations

var boundingBox: NormalizedRect

