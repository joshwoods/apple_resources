

- FSKit
- FSItem
-  FSItem.GetAttributesRequest 

Class

# FSItem.GetAttributesRequest

A request to get attributes from an item.

macOS 15.4+

``` source
class GetAttributesRequest
```

## Overview

Methods that retrieve attributes use this type and inspect the wantedAttributes property to determine which attributes to provide. FSKit calls the isAttributeWanted(_:) method to determine whether the request requires a given attribute.

## Topics

### Inspecting requested attributes

var wantedAttributes: FSItem.Attribute

The attributes requested by the request.

func isAttributeWanted(FSItem.Attribute) -> Bool

A method that indicates whether the request wants given attribute.

struct Attribute

A value that indicates a set of item attributes to get or set.

## Relationships

### Inherits From

- NSObject

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

### Working with attributes

class Attributes

Attributes of an item, such as size, creation and modification times, and user and group identifiers.

class SetAttributesRequest

A request to set attributes on an item.

