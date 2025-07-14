

- MapKit
- MKCircleRenderer
-  strokeStart 

Instance Property

# strokeStart

The unit distance along the circle where the stroke starts.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var strokeStart: CGFloat { get set }
```

## Discussion

Use this property and strokeEnd to render a portion of the line. As a unit distance, strokeStart must be a value between 0 and 1. A unit distance of 0 represents the top of the circle and the stroke draws in a clockwise direction.

## See Also

### Accessing the stroke

var strokeEnd: CGFloat

The unit distance along the circle where the stroke ends.

