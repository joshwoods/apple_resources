

- Foundation
-  NSRangeSpecifier 

Class

# NSRangeSpecifier

A specifier for a range of objects in a container.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSRangeSpecifier
```

## Overview

An `NSRangeSpecifier` object specifies a range (that is, an uninterrupted series) of objects in a container through two delimiting objects. The range is represented by two object specifiers, a start specifier and an end specifier, which can be of any specifier type (such as NSIndexSpecifier or NSWhoseSpecifier object). These specifiers are evaluated in the context of the same container object as the range specifier itself.

You don’t normally subclass `NSRangeSpecifier`.

## Topics

### Initializing a range specifier

init(containerClassDescription: NSScriptClassDescription, containerSpecifier: NSScriptObjectSpecifier?, key: String, start: NSScriptObjectSpecifier?, end: NSScriptObjectSpecifier?)

Returns a range specifier initialized with the given properties.

### Accessing a range specifier

var endSpecifier: NSScriptObjectSpecifier?

Sets the object specifier representing the last object of the range to a given object.

var startSpecifier: NSScriptObjectSpecifier?

Returns the object specifier representing the first object of the range.

### Initializers

init?(coder: NSCoder)

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

class NSUniqueIDSpecifier

A specifier for an object in a collection (or container) by unique ID.

class NSWhoseSpecifier

A specifier that indicates every object in a collection matching a condition.

class NSNameSpecifier

A specifier for an object in a collection (or container) by name.

class NSMiddleSpecifier

A specifier indicating the middle object in a collection or, if not a one-to-many relationship, the sole object.

class NSIndexSpecifier

A specifier representing an object in a collection (or container) with an index number.

class NSRelativeSpecifier

A specifier that indicates an object in a collection by its position relative to another object.

