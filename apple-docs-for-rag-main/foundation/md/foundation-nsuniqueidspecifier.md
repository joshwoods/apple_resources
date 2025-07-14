

- Foundation
-  NSUniqueIDSpecifier 

Class

# NSUniqueIDSpecifier

A specifier for an object in a collection (or container) by unique ID.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSUniqueIDSpecifier
```

## Overview

This specifier works only for objects that have an ID property. The unique ID object passed to an instance of `NSUniqueIDSpecifier` must be either an `NSNumber` object or an `NSString` object. The exact type should match the scripting dictionary declaration of the ID attribute for the relevant scripting class.

You can expect that the ID property will be *read only* for any object that supports it. Therefore a scripter can obtain the unique ID for an object and refer to the object by the ID, but cannot set the unique ID.

You don’t normally subclass `NSUniqueIDSpecifier`.

The evaluation of `NSUniqueIDSpecifier` objects follows these steps until the specified object is found:

1.  If the container implements a method whose selector matches the relevant `valueInWithUniqueID:` pattern established by scripting key-value coding, the method is invoked. This method can potentially be very fast, and it may be relatively easy to implement.

2.  As is the case when evaluating any script object specifier, the container of the specified object is given a chance to evaluate the object specifier. If the container class implements the indicesOfObjects(byEvaluatingObjectSpecifier:) method, the method is invoked. This method can potentially be very fast, but it is relatively difficult to implement.

3.  An NSWhoseSpecifier object that specifies the first object whose relevant `'ID '` attribute matches the ID is synthesized and evaluated. The `NSWhoseSpecifier` object must search through all of the keyed elements in the container, looking for a match. The search is potentially very slow.

## Topics

### Initializing a unique ID specifier

init(containerClassDescription: NSScriptClassDescription, containerSpecifier: NSScriptObjectSpecifier?, key: String, uniqueID: Any)

Returns an `NSUniqueIDSpecifier` object, initialized with the given arguments.

### Accessing unique ID information

var uniqueID: Any

Returns the ID encapsulated by the receiver.

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

