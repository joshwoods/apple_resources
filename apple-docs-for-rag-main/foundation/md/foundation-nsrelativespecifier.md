

- Foundation
-  NSRelativeSpecifier 

Class

# NSRelativeSpecifier

A specifier that indicates an object in a collection by its position relative to another object.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSRelativeSpecifier
```

## Overview

You don’t normally subclass `NSRelativeSpecifier`.

## Topics

### Initializing a relative specifier

init(containerClassDescription: NSScriptClassDescription, containerSpecifier: NSScriptObjectSpecifier?, key: String, relativePosition: NSRelativeSpecifier.RelativePosition, baseSpecifier: NSScriptObjectSpecifier?)

Invokes the super class’s init(containerClassDescription:containerSpecifier:key:) method and initializes the relative position and base specifier to `relPos` and `baseSpecifier`.

### Accessing a relative specifier

var baseSpecifier: NSScriptObjectSpecifier?

Sets the specifier for the base object.

var relativePosition: NSRelativeSpecifier.RelativePosition

Sets the relative position encapsulated by the receiver.

### Constants

enum RelativePosition

These constants are used by relativePosition and relativePosition.

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

class NSIndexSpecifier

A specifier representing an object in a collection (or container) with an index number.

