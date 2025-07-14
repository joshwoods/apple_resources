

- Core Image
- CIFilter
- Transition Filters
-  CIPageCurlTransition 

Protocol

# CIPageCurlTransition

The properties you use to configure a page curl transition filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIPageCurlTransition
```

## Topics

### Instance Properties

var angle: Float

The angle of the curling page.

**Required**

var backsideImage: CIImage?

The image that appears on the back of the source image as the page curls to reveal the target image.

**Required**

var extent: CGRect

The extent of the effect.

**Required**

var radius: Float

The radius of the curl.

**Required**

var shadingImage: CIImage?

An image that looks like a shaded sphere enclosed in a square.

**Required**

## Relationships

### Inherits From

- CITransitionFilter

## See Also

### Related Documentation

class func pageCurlTransition() -> any CIFilter &amp; CIPageCurlTransition

Simulates the curl of a page, revealing the target image.

