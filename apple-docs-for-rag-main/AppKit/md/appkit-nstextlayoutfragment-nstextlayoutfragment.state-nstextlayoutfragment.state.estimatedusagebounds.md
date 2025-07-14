

- AppKit
- NSTextLayoutFragment
- NSTextLayoutFragment.State
-  NSTextLayoutFragment.State.estimatedUsageBounds 

Case

# NSTextLayoutFragment.State.estimatedUsageBounds

The text layout manager hasn’t performed a full layout yet for the region covered by this layout fragment and is returning an estimated bounds.

macOS 12.0+

``` source
case estimatedUsageBounds
```

## See Also

### Constants that describe layout bounds

case calculatedUsageBounds

The layout fragment measurements are available without text line fragments.

case layoutAvailable

Measurements for the text line fragments and layout fragment are available.

case none

No layout information is available.

