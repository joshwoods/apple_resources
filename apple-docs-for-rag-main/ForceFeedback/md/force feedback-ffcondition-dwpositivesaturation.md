

- Force Feedback
- FFCONDITION
-  dwPositiveSaturation 

Instance Property

# dwPositiveSaturation

Maximum force output on the positive side of the offset, in the range from 0 through 10,000.

Mac Catalyst 13.0+macOS 10.2+

``` source
var dwPositiveSaturation: DWORD
```

## Discussion

If the device does not support force saturations, the value of this member is ignored.

## See Also

### Instance Properties

var dwNegativeSaturation: DWORD

Maximum force output on the negative side of the offset, in the range from 0 through 10,000.

var lDeadBand: LONG

Region around **lOffset** in which the condition is not active, in the range from 0 through 10,000. In other words, the condition is not active between **lOffset** minus **lDeadBand** and **lOffset** plus **lDeadBand**.

var lNegativeCoefficient: LONG

Coefficient constant on the negative side of the offset, in the range from -10,000 through 10,000.

var lOffset: LONG

Offset for the condition, in the range from -10,000 through 10,000.

var lPositiveCoefficient: LONG

Coefficient constant on the positive side of the offset, in the range from -10,000 through 10,000.

