

- TV Services
-  TVTopShelfObject 

Class

# TVTopShelfObject

An abstract base class for describing top shelf items and item collections.

tvOS 13.0+

``` source
class TVTopShelfObject
```

## Overview

This class provides shared information for objects you use in your app extension. Do not create instances of this class directly.

## Topics

### Getting the Object Attributes

var title: String?

The localized title of the object.

## Relationships

### Inherits From

- NSObject

### Inherited By

- TVTopShelfItem
- TVTopShelfItemCollection

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

class TVTopShelfAction

An action to perform in response to user interactions with an item in the top shelf.

protocol TVTopShelfContent

The protocol that objects adopt to provide content for the top shelf.

