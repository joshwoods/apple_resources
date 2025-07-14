

- CarPlay
-  CPInformationItem 

Class

# CPInformationItem

A data object that provides content for an information template.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPInformationItem
```

## Overview

CPInformationTemplate uses information items to populate the rows of its list. Depending on the template’s layout, the item’s title and detail values stack vertically or horizontally in the row. Use the `title` property to describe the content, and the `detail` property to provide the content. For example, when using `CPInformationTemplate` to present a food order summary, you could provide an item that displays the number of minutes until the order is ready.

## Topics

### Creating an Information Item

init(title: String?, detail: String?)

Creates an information item with a title and detail text.

### Accessing the Item’s Attributes

var title: String?

The text that the template displays as the item’s title.

var detail: String?

The text that the template displays below or beside the item’s title.

## Relationships

### Inherits From

- NSObject

### Inherited By

- CPInformationRatingItem

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

class CPInformationRatingItem

A data object that provides rated content for an information template.

