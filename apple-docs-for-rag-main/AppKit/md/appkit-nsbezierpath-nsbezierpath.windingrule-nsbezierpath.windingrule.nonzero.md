

- AppKit
- NSBezierPath
- NSBezierPath.WindingRule
-  NSBezierPath.WindingRule.nonZero 

Case

# NSBezierPath.WindingRule.nonZero

Specifies the non-zero winding rule.

macOS

``` source
case nonZero
```

## Discussion

Count each left-to-right path as +1, and each right-to-left path as -1. If the sum of all crossings is 0, the point is outside the path. If the sum is nonzero, the point is inside the path and the region containing it is filled. This is the default winding rule.

## See Also

### Constants

case evenOdd

Specifies the even-odd winding rule.

