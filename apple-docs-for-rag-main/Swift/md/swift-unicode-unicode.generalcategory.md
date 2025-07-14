

- Swift
- Unicode
-  Unicode.GeneralCategory 

Enumeration

# Unicode.GeneralCategory

The most general classification of a Unicode scalar.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum GeneralCategory
```

## Overview

The general category of a scalar is its “first-order, most usual categorization”. It does not attempt to cover multiple uses of some scalars, such as the use of letters to represent Roman numerals.

## Topics

### Operators

static func == (Unicode.GeneralCategory, Unicode.GeneralCategory) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case closePunctuation

A closing punctuation mark of a pair.

case connectorPunctuation

A connecting punctuation mark, like a tie.

case control

A C0 or C1 control code.

case currencySymbol

A currency sign.

case dashPunctuation

A dash or hyphen punctuation mark.

case decimalNumber

A decimal digit.

case enclosingMark

An enclosing combining mark.

case finalPunctuation

A final quotation mark.

case format

A format control character.

case initialPunctuation

An initial quotation mark.

case letterNumber

A letter-like numeric character.

case lineSeparator

A line separator, which is specifically (and only) U+2028 LINE SEPARATOR.

case lowercaseLetter

A lowercase letter.

case mathSymbol

A symbol of mathematical use.

case modifierLetter

A modifier letter.

case modifierSymbol

A non-letterlike modifier symbol.

case nonspacingMark

A non-spacing combining mark with zero advance width (abbreviated Mn).

case openPunctuation

An opening punctuation mark of a pair.

case otherLetter

Other letters, including syllables and ideographs.

case otherNumber

A numeric character of another type.

case otherPunctuation

A punctuation mark of another type.

case otherSymbol

A symbol of another type.

case paragraphSeparator

A paragraph separator, which is specifically (and only) U+2029 PARAGRAPH SEPARATOR.

case privateUse

A private-use character.

case spaceSeparator

A space character of non-zero width.

case spacingMark

A spacing combining mark with positive advance width.

case surrogate

A surrogate code point.

case titlecaseLetter

A digraph character whose first part is uppercase.

case unassigned

A reserved unassigned code point or a non-character.

case uppercaseLetter

An uppercase letter.

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

struct CanonicalCombiningClass

The classification of a scalar used in the Canonical Ordering Algorithm defined by the Unicode Standard.

enum NumericType

The numeric type of a scalar.

