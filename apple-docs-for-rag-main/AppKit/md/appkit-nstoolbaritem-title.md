

- AppKit
- NSToolbarItem
-  title 

Instance Property

# title

The title of the toolbar item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
@MainActor
var title: String { get set }
```

## Discussion

If you assign a custom view to the toolbar item, modifying this property updates the title property of the view if one exists. If the toolbar item contains a button, modifying this property updates the button title. If the item doesn’t contain a custom view, the toolbar item manages the content directly.

Note

In macOS 12 and earlier, NSToolbarItem doesn’t support custom views in Mac apps built with Mac Catalyst.

## See Also

### Describing the item

var possibleLabels: Set&lt;String>

The set of labels that the item might display.

var label: String

The label that appears for this item in the toolbar.

var paletteLabel: String

The label that appears when the toolbar item is in the customization palette.

var toolTip: String?

The tooltip to display when someone hovers over the item in the toolbar.

