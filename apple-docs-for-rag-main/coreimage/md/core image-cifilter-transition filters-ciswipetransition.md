

- Core Image
- CIFilter
- Transition Filters
-  CISwipeTransition 

Protocol

# CISwipeTransition

The properties you use to configure a swipe transition filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CISwipeTransition
```

## Topics

### Instance Properties

var angle: Float

The angle of the swipe.

**Required**

var color: CIColor

The color of the swipe.

**Required**

var extent: CGRect

The extent of the effect.

**Required**

var opacity: Float

The opacity of the swipe.

**Required**

var width: Float

The width of the swipe.

**Required**

## Relationships

### Inherits From

- CITransitionFilter

## See Also

### Related Documentation

class func swipeTransition() -> any CIFilter &amp; CISwipeTransition

Gradually transitions from one image to another with a swiping motion.

