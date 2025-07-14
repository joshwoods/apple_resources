

- AppKit
- NSTextLayoutFragment
- NSTextLayoutFragment.State
-  NSTextLayoutFragment.State.none 

Case

# NSTextLayoutFragment.State.none

No layout information is available.

macOS 12.0+

``` source
case none
```

## See Also

### Constants that describe layout bounds

case calculatedUsageBounds

The layout fragment measurements are available without text line fragments.

case estimatedUsageBounds

The text layout manager hasn’t performed a full layout yet for the region covered by this layout fragment and is returning an estimated bounds.

case layoutAvailable

Measurements for the text line fragments and layout fragment are available.

