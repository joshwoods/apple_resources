

- Core Image
- CIFilter
- Transition Filters
-  CIModTransition 

Protocol

# CIModTransition

The properties you use to configure a mod transition filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIModTransition
```

## Topics

### Instance Properties

var angle: Float

The angle of the mod hole pattern.

**Required**

var center: CGPoint

The x and y position to use as the center of the effect.

**Required**

var compression: Float

The amount of stretching applied to the mod hole pattern.

**Required**

var radius: Float

The radius of the undistorted mod holes in the pattern.

**Required**

## Relationships

### Inherits From

- CITransitionFilter

## See Also

### Related Documentation

class func modTransition() -> any CIFilter &amp; CIModTransition

Transitions between two images by applying irregularly shaped holes.

