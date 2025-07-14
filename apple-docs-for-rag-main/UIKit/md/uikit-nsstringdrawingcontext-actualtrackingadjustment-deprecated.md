

- UIKit
- NSStringDrawingContext
-  actualTrackingAdjustment Deprecated

Instance Property

# actualTrackingAdjustment

The actual tracking value that the system applied during drawing.

watchOS 2.0–2.0Deprecated

``` source
var actualTrackingAdjustment: CGFloat { get }
```

## Discussion

If you specified a custom value in the minimumTrackingAdjustment property, when drawing is complete, this property contains the actual tracking value that was used.

## See Also

### Deprecated

var minimumTrackingAdjustment: CGFloat

The smallest amount of space, in points, to maintain between characters.

Deprecated

