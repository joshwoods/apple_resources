

- TV Services
-  TVTopShelfAction 

Class

# TVTopShelfAction

An action to perform in response to user interactions with an item in the top shelf.

tvOS 13.0+

``` source
class TVTopShelfAction
```

## Overview

A TVTopShelfAction object contains the URL that you want tvOS to open when the user selects an item in the top shelf. Use actions to specify the location of playable content or pages containing additional information.

When configuring a TVTopShelfItem to display in a carousel interface, the system chooses a title and image for each button on the item based on whether you assigned the action object to the playAction or displayAction property of your item.

## Topics

### Creating an Action Object

init(url: URL)

Creates a new action object that displays the content at the specified URL.

### Getting the URL

var url: URL

The URL of the content you want to display.

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

## See Also

### Common types

class TVTopShelfItem

An item that uses an image to represent a movie, show, or other content in the top shelf.

protocol TVTopShelfContent

The protocol that objects adopt to provide content for the top shelf.

class TVTopShelfObject

An abstract base class for describing top shelf items and item collections.

