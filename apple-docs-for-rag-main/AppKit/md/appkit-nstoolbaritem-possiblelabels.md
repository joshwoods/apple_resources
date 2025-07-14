

- AppKit
- NSToolbarItem
-  possibleLabels 

Instance Property

# possibleLabels

The set of labels that the item might display.

iOS 13.0+iPadOS 13.0+Mac Catalyst 16.1+macOS 13.0+

``` source
@MainActor
var possibleLabels: Set { get set }
```

## Discussion

Use this property to specify all of the labels you might possibly use for the toolbar item. Specify all strings in the current locale. To ensure there’s space for the longest label, the item sizes itself using the strings you provide.

## See Also

### Describing the item

var label: String

The label that appears for this item in the toolbar.

var paletteLabel: String

The label that appears when the toolbar item is in the customization palette.

var title: String

The title of the toolbar item.

var toolTip: String?

The tooltip to display when someone hovers over the item in the toolbar.

