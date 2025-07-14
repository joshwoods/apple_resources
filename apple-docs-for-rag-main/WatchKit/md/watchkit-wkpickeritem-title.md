

- WatchKit
- WKPickerItem
-  title 

Instance Property

# title

The text to display for the item.

watchOS 2.0+

``` source
var title: String? { get set }
```

## Discussion

This string contains the item’s content and is displayed when the item is selected. Titles are used for pickers configured to display a list. They are not shown for stack and image sequence styles.

## See Also

### Setting the Picker Item’s Content

var contentImage: WKImage?

The image to display for the item.

var accessoryImage: WKImage?

A small image to display next to the title string.

var caption: String?

A caption for the item’s content.

