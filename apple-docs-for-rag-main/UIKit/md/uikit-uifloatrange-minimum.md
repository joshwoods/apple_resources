

- UIKit
- UIFloatRange
-  minimum 

Instance Property

# minimum

The minimum range of motion for sliding and pin attachments.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
var minimum: CGFloat
```

## Discussion

For sliding attachments, it represents the number of points to move along the axis of translation in the negative direction. For pin attachments, it represents the number of radians to rotate in the counter-clockwise direction. This value must be less than or equal to `0`.

## See Also

### Getting the range values

var maximum: CGFloat

The maximum range of motion for sliding and pin attachments.

