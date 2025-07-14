

- TV Services
-  TVTopShelfContent 

Protocol

# TVTopShelfContent

The protocol that objects adopt to provide content for the top shelf.

tvOS 13.0+

``` source
protocol TVTopShelfContent : NSObjectProtocol
```

## Overview

Don’t adopt this protocol in your own classes. The TVServices framework adopts this protocol in classes that can contain top shelf content, such as the TVTopShelfCarouselContent class.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- TVTopShelfCarouselContent
- TVTopShelfInsetContent
- TVTopShelfSectionedContent

## See Also

### Common types

class TVTopShelfItem

An item that uses an image to represent a movie, show, or other content in the top shelf.

class TVTopShelfAction

An action to perform in response to user interactions with an item in the top shelf.

class TVTopShelfObject

An abstract base class for describing top shelf items and item collections.

