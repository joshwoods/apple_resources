

- UIKit
- UIFloatRange
-  maximum 

Instance Property

# maximum

The maximum range of motion for sliding and pin attachments.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
var maximum: CGFloat
```

## Discussion

For sliding attachments, it represents the number of points to move along the axis of translation in the positive direction. For pin attachments, it represents the number of radians to rotate in the clockwise direction. This value must be greater than or equal to `0`.

## See Also

### Getting the range values

var minimum: CGFloat

The minimum range of motion for sliding and pin attachments.

