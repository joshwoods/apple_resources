

- TV Services
-  TVTopShelfItemCollection 

Class

# TVTopShelfItemCollection

A group of items that you display together in a sectioned interface in the top shelf.

tvOS 13.0+

``` source
class TVTopShelfItemCollection where Item : TVTopShelfItem
```

## Overview

Use a TVTopShelfItemCollection object to organize related groups of items in a sectioned interface. The system presents the items in your collection together, displaying the title of the collection above those items. For example, you might create different collections for new movies, the user’s favorites, and recently watched movies.

## Topics

### Creating an Item Collection

init(items: [Item])

Creates an item collection object from the specified set of top shelf items.

### Getting the Items

var items: [Item]

The items in the collection.

## Relationships

### Inherits From

- TVTopShelfObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Sectioned and inset content

class TVTopShelfSectionedItem

An item to display in a section-based interface.

class TVTopShelfSectionedContent

The set of items you want to present using a section-based interface in the top shelf.

class TVTopShelfInsetContent

A set of items to present using an inset-style interface in the top shelf.

