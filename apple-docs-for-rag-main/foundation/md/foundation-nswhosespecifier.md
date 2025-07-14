

- Foundation
-  NSWhoseSpecifier 

Class

# NSWhoseSpecifier

A specifier that indicates every object in a collection matching a condition.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSWhoseSpecifier
```

## Overview

`NSWhoseSpecifier` specifies every object in a collection (or every element in a container) that matches the condition defined by a single Boolean expression or multiple Boolean expressions connected by logical operators. `NSWhoseSpecifier` is unique among object specifiers in that its top-level container is typically not the application object but an evaluated object specifier involved in the tested-for condition. An `NSWhoseSpecifier` object encapsulates a “test” object for defining this condition. A test object is instantiated from a subclass of the abstract NSScriptWhoseTest class, whose one declared method is isTrue(). See “Boolean Expressions and Logical Operations” in NSScriptObjectSpecifier and the descriptions in NSComparisonMethods and NSScriptingComparisonMethods for more information.

The set of elements specified by an `NSWhoseSpecifier` object can be a subset of those that pass the `NSWhoseSpecifier` object’s test. This subset is specified by the various sub-element properties of the `NSWhoseSpecifier` object . Consider as an example the specifier `paragraphs where color of third word is blue`. This would be represented by an `NSWhoseSpecifier` object that uses a test specifier and another object specifier to identify a subset of the objects with the specified property. That is, the specifier’s property is `paragraphs`; the test specifier is an index specifier with property `words` and `index 3`; and the qualifier is a key value qualifier for key `color` and value `[NSColor blueColor]`. The test object specifier (`word at index 3`) is evaluated for each object (paragraph) using that object as the container; the resulting objects (if any) are tested with the qualifier (`color blue`).

`NSWhoseSpecifier` is part of Cocoa’s built-in script handling. You don’t normally subclass it.

## Topics

### Initializing a whose specifier

init(containerClassDescription: NSScriptClassDescription, containerSpecifier: NSScriptObjectSpecifier?, key: String, test: NSScriptWhoseTest)

Returns an `NSWhoseSpecifier` object initialized with the given attributes.

### Accessing information about a whose specifier

var endSubelementIdentifier: NSWhoseSpecifier.SubelementIdentifier

Sets the end sub-element identifier for the specifier to the value of a given sub-element.

var endSubelementIndex: Int

Sets the index position of the last sub-element within the range of objects being tested that pass the specifier’s test.

var startSubelementIdentifier: NSWhoseSpecifier.SubelementIdentifier

Returns the start sub-element identifier for the receiver.

var startSubelementIndex: Int

Returns the index position of the first sub-element within the range of objects being tested that pass the receiver’s test.

var test: NSScriptWhoseTest

Returns the test object encapsulated by the receiver.

### Constants

enum SubelementIdentifier

`NSWhoseSpecifier` uses these constants to specify sub-elements within the collection of objects being tested that pass the specifier’s test.

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

class NSNameSpecifier

A specifier for an object in a collection (or container) by name.

class NSMiddleSpecifier

A specifier indicating the middle object in a collection or, if not a one-to-many relationship, the sole object.

class NSIndexSpecifier

A specifier representing an object in a collection (or container) with an index number.

class NSRelativeSpecifier

A specifier that indicates an object in a collection by its position relative to another object.

