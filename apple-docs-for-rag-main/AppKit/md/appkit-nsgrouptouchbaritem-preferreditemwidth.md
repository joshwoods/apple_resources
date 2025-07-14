

- AppKit
- NSGroupTouchBarItem
-  preferredItemWidth 

Instance Property

# preferredItemWidth

The preferred width for items in the group when prefersEqualWidths is true.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.13+

``` source
@MainActor
var preferredItemWidth: CGFloat { get set }
```

## Discussion

This is the width that items are set to if there is enough room, and if the items don’t clip.

This value is ignored if it is negative. The default value is `-1`.

## See Also

### Configuring item width

var prefersEqualWidths: Bool

A Boolean value that specifies that items should have equal widths when possible.

