

- WatchKit
-  WKPickerItem 

Class

# WKPickerItem

A single item in a picker interface.

watchOS 2.0+

``` source
class WKPickerItem
```

## Overview

You create picker items yourself and assign them to a WKInterfacePicker object in your interface. For each item, you can specify a title string, an image, or both based on the style of the picker.

The style of the picker determines how you configure the items of that picker:

- List. Items may be configured in one of two ways:

- Specify an image in the contentImage property.

- Specify text in the title property and an optional image in the accessoryImage property.

- Stacked. Configure each item with an image in the contentImage property.

- Image Sequence. Configure each item with an image in the contentImage property.

## Topics

### Setting the Picker Item’s Content

var contentImage: WKImage?

The image to display for the item.

var title: String?

The text to display for the item.

var accessoryImage: WKImage?

A small image to display next to the title string.

var caption: String?

A caption for the item’s content.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Managing the Picker Contents

func setItems([WKPickerItem]?)

Sets the list of items displayed by the picker.

func setSelectedItemIndex(Int)

Selects the specified item in the list.

func setCoordinatedAnimations([any WKInterfaceObject &amp; WKImageAnimatable]?)

Sets the interface objects that should coordinate their own animations with the picker.

