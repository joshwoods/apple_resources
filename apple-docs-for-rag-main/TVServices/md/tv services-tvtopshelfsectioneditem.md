

- TV Services
-  TVTopShelfSectionedItem 

Class

# TVTopShelfSectionedItem

An item to display in a section-based interface.

tvOS 13.0+

``` source
class TVTopShelfSectionedItem
```

## Overview

Create a TVTopShelfSectionedItem object for each item you want to display in the top shelf. Each sectioned item corresponds to one item of your app’s content. For example, a video playback app uses sectioned items to represent movies or shows. Specify the image for the item using the setImageURL(_:for:) method. Use the inherited playAction and displayAction properties to let the system know what to do when the user interacts with the item.

## Topics

### Setting the Image Shape

var imageShape: TVTopShelfSectionedItem.ImageShape

The aspect ratio of the item’s image.

enum ImageShape

Constants indicating the aspect ratio of an image.

### Setting the Playback Progress

var playbackProgress: Double

The percentage of the content that the user has already played, specified as a value between 0.0 and 1.0.

## Relationships

### Inherits From

- TVTopShelfItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Sectioned and inset content

class TVTopShelfItemCollection

A group of items that you display together in a sectioned interface in the top shelf.

class TVTopShelfSectionedContent

The set of items you want to present using a section-based interface in the top shelf.

class TVTopShelfInsetContent

A set of items to present using an inset-style interface in the top shelf.

