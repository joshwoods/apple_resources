

- CarPlay
-  CPInformationRatingItem 

Class

# CPInformationRatingItem

A data object that provides rated content for an information template.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPInformationRatingItem
```

## Overview

`CPInformationRatingItem` provides the ability to display rated content in the rows of an information template. Depending on the template’s layout, the item’s attributes stack vertically or horizontally in the rows. The title property describes the content, and the detail property provides the content. Use the rating and maximumRating properties to display a rating for the content. For example, you could show a service rating when displaying information about a restaurant or café.

The template manages the visual styling of the rating and maximum rating.

## Topics

### Creating a Rating Item

init(rating: NSNumber?, maximumRating: NSNumber?, title: String?, detail: String?)

Creates a rating item with a current and a maximum rating.

### Accessing the Item’s Attributes

var rating: NSNumber?

The current rating that the template displays.

var maximumRating: NSNumber?

The maximum rating that the template displays.

## Relationships

### Inherits From

- CPInformationItem

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

### Managing the Items

var items: [CPInformationItem]

The items that the template displays.

class CPInformationItem

A data object that provides content for an information template.

