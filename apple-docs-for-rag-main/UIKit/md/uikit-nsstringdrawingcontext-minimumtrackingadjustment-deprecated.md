

- UIKit
- NSStringDrawingContext
-  minimumTrackingAdjustment Deprecated

Instance Property

# minimumTrackingAdjustment

The smallest amount of space, in points, to maintain between characters.

watchOS 2.0–2.0Deprecated

``` source
var minimumTrackingAdjustment: CGFloat { get set }
```

## Discussion

Changing the value of this property tells the renderer that it can change the tracking to a value no smaller than the indicated amount. For example, a value of `-0.5` indicates that characters can be tracked closer together by up to half a point. A value of 0 indicates that the standard spacing is used. A typical range of values for this property would be `-0.5` to `0.0`. The default value of this property is `0.0`.

## See Also

### Deprecated

var actualTrackingAdjustment: CGFloat

The actual tracking value that the system applied during drawing.

Deprecated

