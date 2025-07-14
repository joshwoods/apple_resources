

- Swift
- Unicode
-  Unicode.NumericType 

Enumeration

# Unicode.NumericType

The numeric type of a scalar.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum NumericType
```

## Overview

Scalars with a non-nil numeric type include numbers, fractions, numeric superscripts and subscripts, and circled or otherwise decorated number glyphs.

Some letterlike scalars used in numeric systems, such as Greek or Latin letters, do not have a non-nil numeric type, in order to prevent programs from incorrectly interpreting them as numbers in non-numeric contexts.

## Topics

### Operators

static func == (Unicode.NumericType, Unicode.NumericType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case decimal

A digit that is commonly understood to form base-10 numbers.

case digit

A digit that does not meet the requirements of the `decimal` numeric type.

case numeric

A digit that does not meet the requirements of the `decimal` numeric type or a non-digit numeric value.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Unicode Scalar Classifications

enum GeneralCategory

The most general classification of a Unicode scalar.

struct CanonicalCombiningClass

The classification of a scalar used in the Canonical Ordering Algorithm defined by the Unicode Standard.

