

- AppKit
- NSToolbarItem
-  paletteLabel 

Instance Property

# paletteLabel

The label that appears when the toolbar item is in the customization palette.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
var paletteLabel: String { get set }
```

## Discussion

If you support toolbar customizations, you must provide palette labels for your items. In most cases, you can apply the same value to this property and the label property. However, you might use this property to offer a more descriptive string, or to provide a label string when the label property contains an empty string.

## See Also

### Describing the item

var possibleLabels: Set&lt;String>

The set of labels that the item might display.

var label: String

The label that appears for this item in the toolbar.

var title: String

The title of the toolbar item.

var toolTip: String?

The tooltip to display when someone hovers over the item in the toolbar.

