

- AppKit
- NSPopover
-  hasFullSizeContent 

Instance Property

# hasFullSizeContent

A Boolean value that indicates whether the content view of the popover extends into the arrow region.

macOS 14.0+

``` source
@MainActor
var hasFullSizeContent: Bool { get set }
```

## Discussion

Setting the value of this property to true extends the frame of the content view by the height of the arrow region on all four sides of the frame. This causes the contentViewController view to extend to the window’s bounds.

Use the safeAreaLayoutGuide of the contentViewController view to ensure that your content is fully visible and doesn’t become clipped when displayed.

Setting this value to false doesn’t extend the contentViewController view fully into the arrow region. The default value for this property is false.

