

- AppKit
- NSBezierPath
- NSBezierPath.WindingRule
-  NSBezierPath.WindingRule.evenOdd 

Case

# NSBezierPath.WindingRule.evenOdd

Specifies the even-odd winding rule.

macOS

``` source
case evenOdd
```

## Discussion

Count the total number of path crossings. If the number of crossings is even, the point is outside the path. If the number of crossings is odd, the point is inside the path and the region that contains it is filled.

## See Also

### Constants

case nonZero

Specifies the non-zero winding rule.

