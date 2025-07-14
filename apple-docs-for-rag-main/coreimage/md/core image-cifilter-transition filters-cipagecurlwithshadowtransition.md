

- Core Image
- CIFilter
- Transition Filters
-  CIPageCurlWithShadowTransition 

Protocol

# CIPageCurlWithShadowTransition

The properties you use to configure a page-curl-with-shadow transition filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIPageCurlWithShadowTransition
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

var shadowAmount: Float

The strength of the shadow.

**Required**

var shadowExtent: CGRect

The rectagular portion of input image that casts a shadow.

**Required**

var shadowSize: Float

The maximum size, in pixels, of the shadow.

**Required**

## Relationships

### Inherits From

- CITransitionFilter

## See Also

### Related Documentation

class func pageCurlWithShadowTransition() -> any CIFilter &amp; CIPageCurlWithShadowTransition

Simulates the curl of a page, revealing the target image with added shadow.

