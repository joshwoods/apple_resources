

- WatchKit
- WKPickerItem
-  caption 

Instance Property

# caption

A caption for the item’s content.

watchOS 2.0+

``` source
var caption: String? { get set }
```

## Discussion

When the picker’s focus style includes a caption, the picker gets the text for that caption from this property. Captions are a way to identify the meaning of the item’s content. You can also assign the same caption to all of the items in a picker to identify the purpose of the picker itself.

## See Also

### Setting the Picker Item’s Content

var contentImage: WKImage?

The image to display for the item.

var title: String?

The text to display for the item.

var accessoryImage: WKImage?

A small image to display next to the title string.

