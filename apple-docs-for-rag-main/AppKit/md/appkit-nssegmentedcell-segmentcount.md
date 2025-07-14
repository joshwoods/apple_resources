

- AppKit
- NSSegmentedCell
-  segmentCount 

Instance Property

# segmentCount

The number of segments in the segmented control.

macOS

``` source
@MainActor
var segmentCount: Int { get set }
```

## Discussion

This property contains the number of segments the segmented control should have. If this value is less than the number of segments currently in the control, segments are removed from the right of the control. Similarly, if the number is greater than the current number of segments, the new segments are added on the right. This value must be between `0` and `2049`.

## See Also

### Related Documentation

Segmented Control Programming Guide

