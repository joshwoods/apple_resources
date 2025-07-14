

- Core Image
- CIFilter
- Transition Filters
-  CITransitionFilter 

Protocol

# CITransitionFilter

The properties you use to configure a transition filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CITransitionFilter
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var targetImage: CIImage?

The target image for a transition.

**Required**

var time: Float

The parametric time of the transition.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

### Inherited By

- CIAccordionFoldTransition
- CIBarsSwipeTransition
- CICopyMachineTransition
- CIDisintegrateWithMaskTransition
- CIDissolveTransition
- CIFlashTransition
- CIModTransition
- CIPageCurlTransition
- CIPageCurlWithShadowTransition
- CIRippleTransition
- CISwipeTransition

