

- UIKit
- NSTextStorage
-  NSTextStorage.EditActions 

Structure

# NSTextStorage.EditActions

Constants that indicate the types of changes.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
struct EditActions
```

## Overview

These values are also OR’ed together in notifications to inform instances of `NSLayoutManager` was changed—see textStorage(_:edited:range:changeInLength:invalidatedRange:).

## Topics

### Constants

static var editedAttributes: NSTextStorage.EditActions

Attributes were added, removed, or changed.

static var editedCharacters: NSTextStorage.EditActions

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

