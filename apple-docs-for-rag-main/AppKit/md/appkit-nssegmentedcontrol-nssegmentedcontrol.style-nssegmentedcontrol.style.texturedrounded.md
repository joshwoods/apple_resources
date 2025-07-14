

- AppKit
- NSSegmentedControl
- NSSegmentedControl.Style
-  NSSegmentedControl.Style.texturedRounded 

Case

# NSSegmentedControl.Style.texturedRounded

The control is displayed using the textured rounded style. In macOS 10.7 and later, this style uses the artwork defined for NSSegmentedControl.Style.texturedSquare, so you should specify NSSegmentedControl.Style.texturedSquare instead.

macOS 10.5+

``` source
case texturedRounded
```

## See Also

### Constants

case automatic

The appearance of the segmented control is automatically determined based on the type of window in which the control is displayed and the position within the window.

case rounded

The control is displayed using the rounded style.

case roundRect

The control is displayed using the round rect style.

case texturedSquare

The control is displayed using the textured square style.

case capsule

The control is displayed using the capsule style. In macOS 10.7 and later, this style uses the artwork defined for NSSegmentedControl.Style.texturedSquare, so you should specify NSSegmentedControl.Style.texturedSquare instead.

case smallSquare

The control is displayed using the small square style.

case separated

The segments in the control are displayed very close to each other but not touching. For example, Safari in macOS 10.10 and later uses this style for the previous and next page segmented control.

