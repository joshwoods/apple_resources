

- Core Image
- CIFilter
- Transition Filters
-  CIBarsSwipeTransition 

Protocol

# CIBarsSwipeTransition

The properties you use to configure a bars swipe transition filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIBarsSwipeTransition
```

## Topics

### Instance Properties

var angle: Float

The angle, in radians, of the bars.

**Required**

var barOffset: Float

The offset of one bar with respect to another.

**Required**

var width: Float

The width of each bar.

**Required**

## Relationships

### Inherits From

- CITransitionFilter

## See Also

### Related Documentation

class func barsSwipeTransition() -> any CIFilter &amp; CIBarsSwipeTransition

Transitions between two images by removing rectangular portions of an image.

