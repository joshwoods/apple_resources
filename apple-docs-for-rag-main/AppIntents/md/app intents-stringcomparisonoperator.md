

- App Intents
-  StringComparisonOperator 

Enumeration

# StringComparisonOperator

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum StringComparisonOperator
```

## Topics

### Operators

static func == (StringComparisonOperator, StringComparisonOperator) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case contains

case doesNotContain

case hasPrefix

case hasSuffix

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

## See Also

### String comparisons

class HasPrefixComparator

An object that determines whether the value of a string property has the specified prefix.

class HasSuffixComparator

An object that determines whether the value of a string property has the specified suffix.

