

- Foundation
-  NSNameSpecifier 

Class

# NSNameSpecifier

A specifier for an object in a collection (or container) by name.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSNameSpecifier
```

## Overview

As an example, the following script specifies both an application and a window by name. In this script, the named window’s implicitly specified container is the Finder application’s list of open windows.

```
tell application "Finder" -- specifies an application  by name
    close window "Reports" -- specifies a window by name
end tell
```

This specifier works only for objects that have a name property. You don’t normally subclass `NSNameSpecifier`.

The evaluation of an instance of `NSNameSpecifier` follows these steps until the specified object is found:

1.  If the container implements a method whose selector matches the relevant `valueInWithName:` pattern established by scripting key-value coding, the method is invoked. This method can potentially be very fast, and it may be relatively easy to implement.

2.  As is the case when evaluating any script object specifier, the container of the specified object is given a chance to evaluate the object specifier. If the container class implements the `indicesOfObjectsByEvaluatingObjectSpecifier` method, the method is invoked. This method can potentially be very fast, but it is relatively difficult to implement.

3.  An instance of `NSWhoseSpecifier` that specifies the first object whose relevant `'pnam'` attribute matches the name is synthesized and evaluated. The instance of `NSWhoseSpecifier` must search through all of the keyed elements in the container, looking for a match. The search is potentially very slow.

## Topics

### Initializing a name specifier

init(containerClassDescription: NSScriptClassDescription, containerSpecifier: NSScriptObjectSpecifier?, key: String, name: String)

Invokes the super class’s init(containerClassDescription:containerSpecifier:key:) method and then sets the name instance variable to `name`.

### Accessing a name specifier

var name: String

Sets the name encapsulated with the receiver for the specified object in the container.

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

class NSMiddleSpecifier

A specifier indicating the middle object in a collection or, if not a one-to-many relationship, the sole object.

class NSIndexSpecifier

A specifier representing an object in a collection (or container) with an index number.

class NSRelativeSpecifier

A specifier that indicates an object in a collection by its position relative to another object.

