

- Foundation
- ByteCountFormatStyle
-  ByteCountFormatStyle.Attributed 

Structure

# ByteCountFormatStyle.Attributed

A format style that converts byte counts into attributed strings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Attributed
```

## Overview

Use the attributed modifier on a ByteCountFormatStyle to create a format style of this type.

The attributed strings that this fomat style creates contain attributes from the AttributeScopes.FoundationAttributes.NumberFormatAttributes attribute scope. Use these attributes to determine which runs of the attributed string represent different parts of the formatted value.

## Topics

### Customizing style behavior

var style: ByteCountFormatStyle.Style

The semantic style the format style uses to represent a byte count value.

enum Style

The semantic style to use when formatting a byte count value.

### Accessing style properties

var allowedUnits: ByteCountFormatStyle.Units

The units the format style can use to express the byte count.

var spellsOutZero: Bool

A Boolean value that indicates whether the format style should spell out zero-byte values as text.

var includesActualByteCount: Bool

A Boolean value that indicates whether the format style should include the exact byte count, in addition to expressing it in terms of units.

var locale: Locale

The locale to use to format the numeric part of the byte count.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- FormatStyle
- Hashable
- Sendable

## See Also

### Creating attributed strings

var attributed: ByteCountFormatStyle.Attributed

An attributed format style based on the byte count format style.

