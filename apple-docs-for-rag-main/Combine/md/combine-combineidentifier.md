

- Combine
-  CombineIdentifier 

Structure

# CombineIdentifier

A unique identifier for identifying publisher streams.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct CombineIdentifier
```

## Overview

To conform to CustomCombineIdentifierConvertible in a Subscription or Subject that you implement as a structure, create an instance of CombineIdentifier as follows:

```
let combineIdentifier = CombineIdentifier()
```

## Topics

### Creating a Combine Identifier

init()

Creates a unique Combine identifier.

init(AnyObject)

Creates a Combine identifier, using the bit pattern of the provided object.

### Hashing Identifiers

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Providing a Description

var description: String

A textual representation of this instance.

### Comparing Identifiers

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (CombineIdentifier, CombineIdentifier) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable

## See Also

### Debugging Identifiers

protocol CustomCombineIdentifierConvertible

A protocol for uniquely identifying publisher streams.

