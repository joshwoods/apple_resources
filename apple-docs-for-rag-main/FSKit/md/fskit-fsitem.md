

- FSKit
-  FSItem 

Class

# FSItem

A distinct object in a file hierarchy, such as a file, directory, symlink, socket, and more.

macOS 15.4+

``` source
class FSItem
```

## Overview

An `FSItem` is a mostly opaque object, which your file system implementation defines as needed.

The FSItem.Attributes class defines nonatomic properties to support `FSItem` instances. An FSItem.Attributes instance contains a snapshot of the attributes of an `FSItem` at one point in time. The FSItem.Attributes properties have no explicit thread safety provisions, since the operations that either get or set these properties enforce thread safety.

You test an attribute’s validity with the the method isValid(_:). If the value is `true` (Swift) or `YES` (Objective-C), it’s safe to use the attribute.

Methods that get or set an item’s attribute use FSItem.GetAttributesRequest or FSItem.SetAttributesRequest, respectively. Both are subclasses of FSItem.Attributes. An FSItem.GetAttributesRequest contains a wantedAttributes property to indicate the attributes a file system provides for the request. Similarly, FSItem.SetAttributesRequest uses the property consumedAttributes for a file system to signal back which attributes it successfully used.

`FSItem` is the FSKit equivelant of a vnode in the kernel. For every FSKit vnode in the kernel, the `FSModule` hosting the volume has an instantiated `FSItem`.

## Topics

### Identifying an item

enum Identifier

enum ItemType

An enumeration of item types, such as file, directory, or symbolic link.

### Working with attributes

class Attributes

Attributes of an item, such as size, creation and modification times, and user and group identifiers.

class GetAttributesRequest

A request to get attributes from an item.

class SetAttributesRequest

A request to set attributes on an item.

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

