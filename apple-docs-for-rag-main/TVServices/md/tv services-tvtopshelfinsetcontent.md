

- TV Services
-  TVTopShelfInsetContent 

Class

# TVTopShelfInsetContent

A set of items to present using an inset-style interface in the top shelf.

tvOS 13.0+

``` source
class TVTopShelfInsetContent
```

## Overview

Create a TVTopShelfInsetContent object when you want to display your top shelf content using an inset interface. The layout for an inset interface shows a series of large images, each of which spans almost the entire width of the screen. The focused image appears raised above the background.

For more information about how to configure images for an inset interface, see Human Interface Guidelines.

## Topics

### Creating an Inset Content Object

init(items: [TVTopShelfItem])

Creates an inset content object and populates it with the specified set of items.

### Getting the Items

var items: [TVTopShelfItem]

The items to display from the inset interface.

### Getting the Image Size

class var imageSize: CGSize

The standard width and height for images in an inset interface.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- TVTopShelfContent

## See Also

### Sectioned and inset content

class TVTopShelfSectionedItem

An item to display in a section-based interface.

class TVTopShelfItemCollection

A group of items that you display together in a sectioned interface in the top shelf.

class TVTopShelfSectionedContent

The set of items you want to present using a section-based interface in the top shelf.

