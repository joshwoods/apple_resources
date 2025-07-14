

- WatchKit
- WKPickerItem
-  accessoryImage 

Instance Property

# accessoryImage

A small image to display next to the title string.

watchOS 2.0+

``` source
@NSCopying
var accessoryImage: WKImage? { get set }
```

## Discussion

The dimensions of an accessory image are 13 points wide by 13 points high. Larger images are scaled and centered to fit the available space. Smaller images are centered but not scaled.

## See Also

### Setting the Picker Item’s Content

var contentImage: WKImage?

The image to display for the item.

var title: String?

The text to display for the item.

var caption: String?

A caption for the item’s content.

