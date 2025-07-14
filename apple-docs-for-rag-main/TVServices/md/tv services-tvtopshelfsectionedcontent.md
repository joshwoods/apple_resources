

- TV Services
-  TVTopShelfSectionedContent 

Class

# TVTopShelfSectionedContent

The set of items you want to present using a section-based interface in the top shelf.

tvOS 13.0+

``` source
class TVTopShelfSectionedContent
```

## Overview

Create a TVTopShelfSectionedContent object when you want to display your top shelf content using a sectioned interface. A sectioned interface displays a single labled row of items. Items are organized by section. As the row scrolls horizontally through the items, the system updates the label above the items to indicate the current section. You specify the title of each section and its items using TVTopShelfItemCollection objects.

For more information about how to configure images for a sectioned interface, see Human Interface Guidelines.

## Topics

### Creating a Sectioned Content Object

init(sections: [TVTopShelfItemCollection&lt;TVTopShelfSectionedItem>])

Creates a sectioned content object and populates it with the specified sections.

### Getting the Sections

var sections: [TVTopShelfItemCollection&lt;TVTopShelfSectionedItem>]

The sections to display in the interface.

### Getting the Image Size Information

class func imageSize(for: TVTopShelfSectionedItem.ImageShape) -> CGSize

Returns the dimensions to use for images of the specified shape.

enum ImageShape

Constants indicating the aspect ratio of an image.

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

class TVTopShelfInsetContent

A set of items to present using an inset-style interface in the top shelf.

