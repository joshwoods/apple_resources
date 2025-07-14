

- Core Image
- CIFilter
- Transition Filters
-  CIAccordionFoldTransition 

Protocol

# CIAccordionFoldTransition

The properties you use to configure an accordion fold transition filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIAccordionFoldTransition
```

## Topics

### Instance Properties

var bottomHeight: Float

The height of the accordion-fold part of the transition.

**Required**

var foldShadowAmount: Float

A value that specifies the intensity of the shadow in the transtion.

**Required**

var numberOfFolds: Float

The number of folds used in the transition.

**Required**

## Relationships

### Inherits From

- CITransitionFilter

## See Also

### Related Documentation

class func accordionFoldTransition() -> any CIFilter &amp; CIAccordionFoldTransition

Transitions by folding and crossfading an image to reveal the target image.

