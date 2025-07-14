

- FSKit
- FSItem
-  FSItem.SetAttributesRequest 

Class

# FSItem.SetAttributesRequest

A request to set attributes on an item.

macOS 15.4+

``` source
class SetAttributesRequest
```

## Overview

Methods that take attributes use this type to receive attribute values and to indicate which attributes they support. The various members of the parent type, FSItem.Attributes, contain the values of the attributes to set.

Modify the consumedAttributes property to indicate which attributes your file system successfully used. FSKit calls the wasAttributeConsumed(_:) method to determine whether the file system successfully used a given attribute. Only set the attributes that your file system supports.

## Topics

### Inspecting used attributes

var consumedAttributes: FSItem.Attribute

The attributes successfully used by the file system.

func wasAttributeConsumed(FSItem.Attribute) -> Bool

A method that indicates whether the file system used the given attribute.

struct Attribute

A value that indicates a set of item attributes to get or set.

## Relationships

### Inherits From

- FSItem.Attributes

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

class GetAttributesRequest

A request to get attributes from an item.

