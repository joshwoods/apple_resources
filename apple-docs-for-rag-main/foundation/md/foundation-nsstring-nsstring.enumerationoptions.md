

- Foundation
- NSString
-  NSString.EnumerationOptions 

Structure

# NSString.EnumerationOptions

Constants to specify kinds of substrings and styles of enumeration.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct EnumerationOptions
```

## Overview

These options are used with the enumerateSubstrings(in:options:using:) method. Pass in one `NSStringEnumerationBy...` option and combine with any of the remaining enumeration style constants using the C bitwise `OR` operator.

## Topics

### Constants

static var byLines: NSString.EnumerationOptions

static var byParagraphs: NSString.EnumerationOptions

static var byComposedCharacterSequences: NSString.EnumerationOptions

static var byWords: NSString.EnumerationOptions

static var bySentences: NSString.EnumerationOptions

static var reverse: NSString.EnumerationOptions

static var substringNotRequired: NSString.EnumerationOptions

static var localized: NSString.EnumerationOptions

static var byLines: NSString.EnumerationOptions

static var byParagraphs: NSString.EnumerationOptions

static var byComposedCharacterSequences: NSString.EnumerationOptions

static var byWords: NSString.EnumerationOptions

static var bySentences: NSString.EnumerationOptions

static var reverse: NSString.EnumerationOptions

static var substringNotRequired: NSString.EnumerationOptions

static var localized: NSString.EnumerationOptions

### Initializers

init(rawValue: UInt)

### Type Properties

static var byCaretPositions: NSString.EnumerationOptions

static var byDeletionClusters: NSString.EnumerationOptions

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Performing Linguistic Analysis

func enumerateLinguisticTags(in: NSRange, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, orthography: NSOrthography?, using: (NSLinguisticTag?, NSRange, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Performs linguistic analysis on the specified string by enumerating the specific range of the string, providing the Block with the located tags.

Deprecated

func linguisticTags(in: NSRange, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, orthography: NSOrthography?, tokenRanges: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> [NSLinguisticTag]

Returns an array of linguistic tags for the specified range and requested tags within the receiving string.

Deprecated

