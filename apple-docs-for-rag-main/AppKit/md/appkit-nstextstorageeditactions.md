

- AppKit
-  NSTextStorageEditActions 

Structure

# NSTextStorageEditActions

Constants that indicate the types of changes.

macOS 10.11+

``` source
struct NSTextStorageEditActions
```

## Overview

These values are also OR’ed together in notifications to inform instances of `NSLayoutManager` was changed—see textStorage(_:edited:range:changeInLength:invalidatedRange:).

## Topics

### Constants

static var editedAttributes: NSTextStorageEditActions

Attributes were added, removed, or changed.

static var editedCharacters: NSTextStorageEditActions

Characters were added, removed, or replaced.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

