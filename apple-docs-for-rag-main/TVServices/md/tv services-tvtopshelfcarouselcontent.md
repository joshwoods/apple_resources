

- TV Services
-  TVTopShelfCarouselContent 

Class

# TVTopShelfCarouselContent

A set of items you present using a carousel-style interface in the top shelf.

tvOS 13.0+

``` source
class TVTopShelfCarouselContent
```

## Topics

### Creating a Carousel Content Object

init(style: TVTopShelfCarouselContent.Style, items: [TVTopShelfCarouselItem])

Creates a content object for displaying items in a carousel style in the top shelf interface.

### Accessing the Carousel Items

var items: [TVTopShelfCarouselItem]

The items to display in the top shelf interface.

### Getting the Item Style

var style: TVTopShelfCarouselContent.Style

The appearance to use when displaying items in the top shelf interface.

enum Style

Constants indicating how you want items to appear in the top shelf interface.

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

### Carousel content

class TVTopShelfCarouselItem

An item containing images, video, and other information that you want to display using a carousel-based interface.

