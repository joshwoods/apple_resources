

- Core Data
-  NSDerivedAttributeDescription 

Class

# NSDerivedAttributeDescription

A description of an attribute that derives its value by performing a calculation on a related attribute.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class NSDerivedAttributeDescription
```

## Overview

Use derived attributes to optimize fetch performance; for example:

- Create a derived `searchName` attribute to reflect a `name` attribute with case and diacritics removed for more efficient comparison.

- Create a derived `relationshipCount` attribute to reflect the number of objects in a relationship and avoid having to do a join.

Derived attributes support the following expressions:

| **Expression** | **Description** | **Example** |
|----|----|----|
| to-one keypath | A single value to replicate. | `name` or `author.name` |
| to-one keypath with a function | The result of calling a function on a single value.  Supported functions include `canonical:`, `uppercase:`, and `lowercase:`.  The `canonical:` function returns a case- and diacritic-insensitive String value. | `canonical:(name)` |
| to-many keypath with a function | The result of calling an aggregate function on a set of values.  Supported functions include `@count` and `@sum`. | `friends.@count` |
| time | The current time. | `now()` |

Important

Data recomputes derived attributes when you save a context. A managed object’s property does not reflect unsaved changes until you save the context and refresh the object.

## Topics

### Specifying the Derivation Expression

var derivationExpression: NSExpression?

An expression for generating derived data.

## Relationships

### Inherits From

- NSAttributeDescription

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Computed attributes

class NSCompositeAttributeDescription

A description of an attribute that derives its value by composing other attributes.

