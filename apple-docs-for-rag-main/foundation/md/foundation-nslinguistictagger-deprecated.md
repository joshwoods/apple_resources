

- Foundation
-  NSLinguisticTagger Deprecated

Class

# NSLinguisticTagger

Analyze natural language text to tag part of speech and lexical class, identify names, perform lemmatization, and determine the language and script.

iOS 5.0–18.4DeprecatediPadOS 5.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.7–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
class NSLinguisticTagger
```

Deprecated

Use the Natural Language framework instead.

## Mentioned in 

Tokenizing Natural Language Text

Identifying Parts of Speech

Identifying People, Places, and Organizations

## Overview

NSLinguisticTagger provides a uniform interface to a variety of natural language processing functionality with support for many different languages and scripts. You can use this class to segment natural language text into paragraphs, sentences, or words, and tag information about those segments, such as part of speech, lexical class, lemma, script, and language.

When you create a linguistic tagger, you specify what kind of information you’re interested in by passing one or more NSLinguisticTagScheme values. Set the string property to the natural language text you want to analyze, and the linguistic tagger processes it according to the specified tag schemes. You can then enumerate over the tags in a specified range, using the methods described in Enumerating Linguistic Tags, to get the information requested for a given scheme and unit.

### Thread Safety

A single instance of NSLinguisticTagger should not be used simultaneously from multiple threads.

## Topics

### First Steps

Tokenizing Natural Language Text

Enumerate the words in a string.

init(tagSchemes: [NSLinguisticTagScheme], options: Int)

Creates a linguistic tagger instance using the specified tag schemes and options.

var string: String?

The string being analyzed by the linguistic tagger.

### Getting the Tag Schemes

class func availableTagSchemes(for: NSLinguisticTaggerUnit, language: String) -> [NSLinguisticTagScheme]

Returns the tag schemes available for a particular unit and language on the current device.

class func availableTagSchemes(forLanguage: String) -> [NSLinguisticTagScheme]

Returns the tag schemes available for a particular language on the current device.

var tagSchemes: [NSLinguisticTagScheme]

Returns the tag schemes configured for this linguistic tagger. For possible values, see NSLinguisticTagScheme.

### Determining the Dominant Language and Orthography

class func dominantLanguage(for: String) -> String?

Returns the dominant language for the specified string.

var dominantLanguage: String?

Returns the dominant language of the string set for the linguistic tagger.

func orthography(at: Int, effectiveRange: NSRangePointer?) -> NSOrthography?

Returns the orthography at the index and also returns the effective range.

func setOrthography(NSOrthography?, range: NSRange)

Sets the orthography for the specified range.

### Enumerating Linguistic Tags

Identifying Parts of Speech

Classify nouns, verbs, adjectives, and other parts of speech in a string.

Identifying People, Places, and Organizations

Use a linguistic tagger to perform named entity recognition on a string.

func enumerateTags(in: NSRange, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, using: (NSLinguisticTag?, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates over a given range of the string for a particular unit and calls the specified block for each tag.

func enumerateTags(in: NSRange, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, using: (NSLinguisticTag?, NSRange, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates over a given range of the string and calls the specified block for each tag.

class func enumerateTags(for: String, range: NSRange, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, orthography: NSOrthography?, using: (NSLinguisticTag?, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates over a given string and calls the specified block for each tag.

struct Options

Constants for linguistic tagger enumeration specifying which tokens to omit and whether to join names.

### Getting Linguistic Tags

func tag(at: Int, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, tokenRange: NSRangePointer?) -> NSLinguisticTag?

Returns a tag for a single scheme, for a given linguistic unit, at the specified character position.

func tag(at: Int, scheme: NSLinguisticTagScheme, tokenRange: NSRangePointer?, sentenceRange: NSRangePointer?) -> NSLinguisticTag?

Returns a tag for a single scheme at the specified character position.

class func tag(for: String, at: Int, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, orthography: NSOrthography?, tokenRange: NSRangePointer?) -> NSLinguisticTag?

Returns a tag for a single scheme, for a given linguistic unit, at the specified character position in a string.

func tags(in: NSRange, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, tokenRanges: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> [NSLinguisticTag]

Returns an array of linguistic tags and token ranges for a given string range and linguistic unit.

func tags(in: NSRange, scheme: String, options: NSLinguisticTagger.Options, tokenRanges: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> [String]

Returns an array of linguistic tags and token ranges for a given string range.

class func tags(for: String, range: NSRange, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, orthography: NSOrthography?, tokenRanges: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> [NSLinguisticTag]

Returns an array of linguistic tags and token ranges for a given string and linguistic unit.

### Determining the Range of a Unit Token

func tokenRange(at: Int, unit: NSLinguisticTaggerUnit) -> NSRange

Returns the range of the linguistic unit containing the specified character index.

func sentenceRange(for: NSRange) -> NSRange

Returns the range of a sentence containing the specified range.

### Determining the Possible Tags

func possibleTags(at: Int, scheme: String, tokenRange: NSRangePointer?, sentenceRange: NSRangePointer?, scores: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> [String]?

Returns an array of possible tags for the given scheme at the specified range, supplying matching scores.

### Notifying for Changes to the Analyzed String

func stringEdited(in: NSRange, changeInLength: Int)

Notifies the linguistic tagger that the string (if mutable) has changed as specified by the parameters.

### Supporting Types

struct NSLinguisticTagScheme

Constants for the tag schemes specified when initializing a linguistic tagger.

enum NSLinguisticTaggerUnit

Constants representing linguistic units.

struct NSLinguisticTag

A token, lexical class, name, lemma, language, or script returned by a linguistic tagger for natural language text.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Deprecated

Deprecated String Encodings

