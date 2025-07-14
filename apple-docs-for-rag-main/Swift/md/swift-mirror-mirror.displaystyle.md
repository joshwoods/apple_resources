

- Swift
- Mirror
-  Mirror.DisplayStyle 

Enumeration

# Mirror.DisplayStyle

A suggestion of how a mirror’s subject is to be interpreted.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum DisplayStyle
```

## Overview

Playgrounds and the debugger will show a representation similar to the one used for instances of the kind indicated by the `DisplayStyle` case name when the mirror is used for display.

## Topics

### Operators

static func == (Mirror.DisplayStyle, Mirror.DisplayStyle) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case `class`

case collection

case dictionary

case `enum`

case optional

case set

case `struct`

case tuple

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

