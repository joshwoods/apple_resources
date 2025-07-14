

- Foundation
- NSLinguisticTagger
-  enumerateTags(for:range:unit:scheme:options:orthography:using:) Deprecated

Type Method

# enumerateTags(for:range:unit:scheme:options:orthography:using:)

Enumerates over a given string and calls the specified block for each tag.

iOS 11.0–18.4DeprecatediPadOS 11.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.13–15.4DeprecatedtvOS 11.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 4.0–9.0Deprecated

``` source
class func enumerateTags(
    for string: String,
    range: NSRange,
    unit: NSLinguisticTaggerUnit,
    scheme: NSLinguisticTagScheme,
    options: NSLinguisticTagger.Options = [],
    orthography: NSOrthography?,
    using block: (NSLinguisticTag?, NSRange, UnsafeMutablePointer) -> Void
)
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Parameters 

`string`  

The string to enumerate over.

`range`  

The range to analyze.

`unit`  

The linguistic unit. For possible values, see NSLinguisticTaggerUnit

`scheme`  

The tag scheme. For possible values, see NSLinguisticTagScheme.

`options`  

The linguistic tagger options to use. See NSLinguisticTagger.Options for possible values.

`orthography`  

The orthography of the string. If unspecified, the orthography is automatically detected.

`block`  

The block to apply to ranges of the string.

The block takes the following arguments:

tag  
The located linguistic tag.

tokenRange  
The range of the linguistic tag.

stop  
A reference to a Boolean value. The block can set the value to true to stop further processing of the set. The `stop` argument is an out-only argument. You should only ever set this Boolean to true within the block.

## Discussion

This method’s block is called for all tokens intersecting a given range, supplying tags and ranges. The tagger segments the string into sentences and tokens as necessary, and return those ranges along with a tag for any scheme in its array of tag schemes. For example, if the tag scheme is lexicalClass, the tags specify the part of speech (for word tokens) or the type of whitespace or punctuation (for whitespace or punctuation tokens). If the tag scheme is lemma, the tags specify the stem form of the word (if known) for each word token.

Important

This method enumerates over the ranges of all tokens that intersect the specified range.

This is a convenience method for initializing a linguistic tagger, setting the string property, and calling the enumerateTags(in:unit:scheme:options:using:) method. If you analyze the same string more than once, you should create a linguistic tagger object instead of calling this method.

## See Also

### Enumerating Linguistic Tags

Identifying Parts of Speech

Classify nouns, verbs, adjectives, and other parts of speech in a string.

Identifying People, Places, and Organizations

Use a linguistic tagger to perform named entity recognition on a string.

func enumerateTags(in: NSRange, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, using: (NSLinguisticTag?, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates over a given range of the string for a particular unit and calls the specified block for each tag.

Deprecated

func enumerateTags(in: NSRange, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, using: (NSLinguisticTag?, NSRange, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates over a given range of the string and calls the specified block for each tag.

Deprecated

struct Options

Constants for linguistic tagger enumeration specifying which tokens to omit and whether to join names.

