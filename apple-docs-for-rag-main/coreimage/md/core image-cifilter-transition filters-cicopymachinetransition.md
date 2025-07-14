

- Core Image
- CIFilter
- Transition Filters
-  CICopyMachineTransition 

Protocol

# CICopyMachineTransition

The properties you use to configure a copy machine transition filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CICopyMachineTransition
```

## Topics

### Instance Properties

var angle: Float

The angle of the copier light.

**Required**

var color: CIColor

The color of the copier light.

**Required**

var extent: CGRect

A rectangle that defines the extent of the effect.

**Required**

var opacity: Float

The opacity of the copier light.

**Required**

var width: Float

The width of the copier light.

**Required**

## Relationships

### Inherits From

- CITransitionFilter

## See Also

### Related Documentation

class func copyMachineTransition() -> any CIFilter &amp; CICopyMachineTransition

Simulates the effect of a copy machine scanner light to transiton between two images.

