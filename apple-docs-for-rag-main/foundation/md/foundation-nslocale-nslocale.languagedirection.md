

- Foundation
- NSLocale
-  NSLocale.LanguageDirection 

Enumeration

# NSLocale.LanguageDirection

The directions that a language may take across a page of text.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum LanguageDirection
```

## Overview

Use these constants with the methods lineDirection(forLanguage:) and characterDirection(forLanguage:).

## Topics

### Constants

case unknown

The direction of the language is unknown.

case leftToRight

The language direction is from left to right.

case rightToLeft

The language direction is from right to left.

case topToBottom

The language direction is from top to bottom.

case bottomToTop

The language direction is from bottom to top.

case unknown

The direction of the language is unknown.

case leftToRight

The language direction is from left to right.

case rightToLeft

The language direction is from right to left.

case topToBottom

The language direction is from top to bottom.

case bottomToTop

The language direction is from bottom to top.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting line and character direction for a language

static func characterDirection(forLanguage: String) -> Locale.LanguageDirection

Returns the character direction for a specified language code.

Deprecated

static func lineDirection(forLanguage: String) -> Locale.LanguageDirection

Returns the line direction for a specified language code.

Deprecated

typealias LanguageDirection

An alias for the standard set of language directions.

