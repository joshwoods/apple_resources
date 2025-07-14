

- AppKit
- NSGroupTouchBarItem
-  prefersEqualWidths 

Instance Property

# prefersEqualWidths

A Boolean value that specifies that items should have equal widths when possible.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.13+

``` source
@MainActor
var prefersEqualWidths: Bool { get set }
```

## Discussion

When true, items in the groupTouchBar are sized to have equal widths when possible.

The default value is false.

## See Also

### Configuring item width

var preferredItemWidth: CGFloat

The preferred width for items in the group when prefersEqualWidths is true.

