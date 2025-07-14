

- Swift
- Unicode
- Unicode.Scalar
-  Unicode.Scalar.Properties 

Structure

# Unicode.Scalar.Properties

A value that provides access to properties of a Unicode scalar that are defined by the Unicode standard.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Properties
```

## Topics

### Instance Properties

var age: Unicode.Version?

The earliest version of the Unicode Standard in which the scalar was assigned.

var canonicalCombiningClass: Unicode.CanonicalCombiningClass

The canonical combining class of the scalar.

var changesWhenCaseFolded: Bool

A Boolean value indicating whether the scalar’s normalized form differs from the case-fold mapping of each constituent scalar.

var changesWhenCaseMapped: Bool

A Boolean value indicating whether the scalar may change when it undergoes case mapping.

var changesWhenLowercased: Bool

A Boolean value indicating whether the scalar’s normalized form differs from the `lowercaseMapping` of each constituent scalar.

var changesWhenNFKCCaseFolded: Bool

A Boolean value indicating whether the scalar is one that is not identical to its NFKC case-fold mapping.

var changesWhenTitlecased: Bool

A Boolean value indicating whether the scalar’s normalized form differs from the `titlecaseMapping` of each constituent scalar.

var changesWhenUppercased: Bool

A Boolean value indicating whether the scalar’s normalized form differs from the `uppercaseMapping` of each constituent scalar.

var generalCategory: Unicode.GeneralCategory

The general category (most usual classification) of the scalar.

var isASCIIHexDigit: Bool

A Boolean value indicating whether the scalar is an ASCII character commonly used for the representation of hexadecimal numbers.

var isAlphabetic: Bool

A Boolean value indicating whether the scalar is alphabetic.

var isBidiControl: Bool

A Boolean value indicating whether the scalar is a format control character that has a specific function in the Unicode Bidirectional Algorithm.

var isBidiMirrored: Bool

A Boolean value indicating whether the scalar is mirrored in bidirectional text.

var isCaseIgnorable: Bool

A Boolean value indicating whether the scalar is ignored for casing purposes.

var isCased: Bool

A Boolean value indicating whether the scalar is considered to be either lowercase, uppercase, or titlecase.

var isDash: Bool

A Boolean value indicating whether the scalar is a punctuation symbol explicitly called out as a dash in the Unicode Standard or a compatibility equivalent.

var isDefaultIgnorableCodePoint: Bool

A Boolean value indicating whether the scalar is a default-ignorable code point.

var isDeprecated: Bool

A Boolean value indicating whether the scalar is deprecated.

var isDiacritic: Bool

A Boolean value indicating whether the scalar is a diacritic.

var isEmoji: Bool

A Boolean value indicating whether the scalar has an emoji presentation, whether or not it is the default.

var isEmojiModifier: Bool

A Boolean value indicating whether the scalar is one that can modify a base emoji that precedes it.

var isEmojiModifierBase: Bool

A Boolean value indicating whether the scalar is one whose appearance can be changed by an emoji modifier that follows it.

var isEmojiPresentation: Bool

A Boolean value indicating whether the scalar is one that should be rendered with an emoji presentation, rather than a text presentation, by default.

var isExtender: Bool

A Boolean value indicating whether the scalar’s principal function is to extend the value or shape of a preceding alphabetic scalar.

var isFullCompositionExclusion: Bool

A Boolean value indicating whether the scalar is excluded from composition when performing Unicode normalization.

var isGraphemeBase: Bool

A Boolean value indicating whether the scalar is a grapheme base.

var isGraphemeExtend: Bool

A Boolean value indicating whether the scalar is a grapheme extender.

var isHexDigit: Bool

A Boolean value indicating whether the scalar is one that is commonly used for the representation of hexadecimal numbers or a compatibility equivalent.

var isIDContinue: Bool

A Boolean value indicating whether the scalar is one which is recommended to be allowed to appear in a non-starting position in a programming language identifier.

var isIDSBinaryOperator: Bool

A Boolean value indicating whether the scalar is an ideographic description character that determines how the two ideographic characters or ideographic description sequences that follow it are to be combined to form a single character.

var isIDSTrinaryOperator: Bool

A Boolean value indicating whether the scalar is an ideographic description character that determines how the three ideographic characters or ideographic description sequences that follow it are to be combined to form a single character.

var isIDStart: Bool

A Boolean value indicating whether the scalar is one which is recommended to be allowed to appear in a starting position in a programming language identifier.

var isIdeographic: Bool

A Boolean value indicating whether the scalar is considered to be a CJKV (Chinese, Japanese, Korean, and Vietnamese) or other siniform (Chinese writing-related) ideograph.

var isJoinControl: Bool

A Boolean value indicating whether the scalar is a format control character that has a specific function in controlling cursive joining and ligation.

var isLogicalOrderException: Bool

A Boolean value indicating whether the scalar requires special handling for operations involving ordering, such as sorting and searching.

var isLowercase: Bool

A Boolean value indicating whether the scalar’s letterform is considered lowercase.

var isMath: Bool

A Boolean value indicating whether the scalar is one that naturally appears in mathematical contexts.

var isNoncharacterCodePoint: Bool

A Boolean value indicating whether the scalar is permanently reserved for internal use.

var isPatternSyntax: Bool

A Boolean value indicating whether the scalar is recommended to have syntactic usage in patterns represented in source code.

var isPatternWhitespace: Bool

A Boolean value indicating whether the scalar is recommended to be treated as whitespace when parsing patterns represented in source code.

var isQuotationMark: Bool

A Boolean value indicating whether the scalar is one that is used in writing to surround quoted text.

var isRadical: Bool

A Boolean value indicating whether the scalar is a radical component of CJK characters, Tangut characters, or Yi syllables.

var isSentenceTerminal: Bool

A Boolean value indicating whether the scalar is a punctuation mark that generally marks the end of a sentence.

var isSoftDotted: Bool

A Boolean value indicating whether the scalar has a “soft dot” that disappears when a diacritic is placed over the scalar.

var isTerminalPunctuation: Bool

A Boolean value indicating whether the scalar is a punctuation symbol that typically marks the end of a textual unit.

var isUnifiedIdeograph: Bool

A Boolean value indicating whether the scalar is one of the unified CJK ideographs in the Unicode Standard.

var isUppercase: Bool

A Boolean value indicating whether the scalar’s letterform is considered uppercase.

var isVariationSelector: Bool

A Boolean value indicating whether the scalar is a variation selector.

var isWhitespace: Bool

A Boolean value indicating whether the scalar is a whitespace character.

var isXIDContinue: Bool

A Boolean value indicating whether the scalar is one which is recommended to be allowed to appear in a non-starting position in a programming language identifier, with adjustments made for NFKC normalized form.

var isXIDStart: Bool

A Boolean value indicating whether the scalar is one which is recommended to be allowed to appear in a starting position in a programming language identifier, with adjustments made for NFKC normalized form.

var lowercaseMapping: String

The lowercase mapping of the scalar.

var name: String?

The published name of the scalar.

var nameAlias: String?

The normative formal alias of the scalar.

var numericType: Unicode.NumericType?

The numeric type of the scalar.

var numericValue: Double?

The numeric value of the scalar.

var titlecaseMapping: String

The titlecase mapping of the scalar.

var uppercaseMapping: String

The uppercase mapping of the scalar.

## Relationships

### Conforms To

- Sendable

## See Also

### Inspecting a Scalar

var value: UInt32

A numeric representation of the Unicode scalar.

var properties: Unicode.Scalar.Properties

Properties of this scalar defined by the Unicode standard.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var isASCII: Bool

A Boolean value indicating whether the Unicode scalar is an ASCII character.

