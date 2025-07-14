

- UIKit
- NSTextLayoutFragment
- NSTextLayoutFragment.State
-  NSTextLayoutFragment.State.layoutAvailable 

Case

# NSTextLayoutFragment.State.layoutAvailable

Measurements for the text line fragments and layout fragment are available.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
case layoutAvailable
```

## See Also

### Constants that describe layout bounds

case calculatedUsageBounds

The layout fragment measurements are available without text line fragments.

case estimatedUsageBounds

The text layout manager hasn’t performed a full layout yet for the region covered by this layout fragment and is returning an estimated bounds.

case none

No layout information is available.

