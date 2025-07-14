

- Foundation
-  NSIndexSpecifier 

Class

# NSIndexSpecifier

A specifier representing an object in a collection (or container) with an index number.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSIndexSpecifier
```

## Overview

The script terms `first` and `front` specify the object with index `0`, while `last` specifies the object with index of `count-1`. A negative index indicates a location by counting backward from the last object in the collection.

You don’t normally subclass `NSIndexSpecifier`.

## Topics

### Creating Index Specifiers

init(containerClassDescription: NSScriptClassDescription, containerSpecifier: NSScriptObjectSpecifier?, key: String, index: Int)

Initializes an allocated NSIndexSpecifier object with a class description, container specifier, collection key, and object index.

### Accessing the Index

var index: Int

Sets the value of the receiver’s `index` property.

## Relationships

### Inherits From

- NSScriptObjectSpecifier

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol

## See Also

### Object Specifiers

class NSScriptObjectSpecifier

An abstract class used to represent natural language expressions.

class NSPropertySpecifier

A specifier for a simple attribute value, a one-to-one relationship, or all elements of a to-many relationship.

class NSPositionalSpecifier

A specifier for an insertion point in a container relative to another object in the container.

class NSRandomSpecifier

A specifier for an arbitrary object in a collection or, if not a one-to-many relationship, the sole object.

class NSRangeSpecifier

A specifier for a range of objects in a container.

class NSUniqueIDSpecifier

A specifier for an object in a collection (or container) by unique ID.

class NSWhoseSpecifier

A specifier that indicates every object in a collection matching a condition.

class NSNameSpecifier

A specifier for an object in a collection (or container) by name.

class NSMiddleSpecifier

A specifier indicating the middle object in a collection or, if not a one-to-many relationship, the sole object.

class NSRelativeSpecifier

A specifier that indicates an object in a collection by its position relative to another object.

