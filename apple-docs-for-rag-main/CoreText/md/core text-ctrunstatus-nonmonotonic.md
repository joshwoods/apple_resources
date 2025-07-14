

- Core Text
- CTRunStatus
-  nonMonotonic 

Type Property

# nonMonotonic

The run isn’t in strictly increasing or decreasing order.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var nonMonotonic: CTRunStatus { get }
```

## Discussion

The run is reordered so that the string indices associated with the glyphs aren’t in strictly increasing (for left-to-right runs) or decreasing (for right-to-left runs) order.

## See Also

### Constants

static var rightToLeft: CTRunStatus

The run proceeds from right to left.

static var hasNonIdentityMatrix: CTRunStatus

The run requires a specific text matrix to be set in the current Core Graphics context for proper drawing.

