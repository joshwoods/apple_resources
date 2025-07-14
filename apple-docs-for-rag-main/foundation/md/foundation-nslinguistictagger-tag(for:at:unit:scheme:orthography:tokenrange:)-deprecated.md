

- Foundation
- NSLinguisticTagger
-  tag(for:at:unit:scheme:orthography:tokenRange:) Deprecated

Type Method

# tag(for:at:unit:scheme:orthography:tokenRange:)

Returns a tag for a single scheme, for a given linguistic unit, at the specified character position in a string.

iOS 11.0–18.4DeprecatediPadOS 11.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.13–15.4DeprecatedtvOS 11.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 4.0–9.0Deprecated

``` source
class func tag(
    for string: String,
    at charIndex: Int,
    unit: NSLinguisticTaggerUnit,
    scheme: NSLinguisticTagScheme,
    orthography: NSOrthography?,
    tokenRange: NSRangePointer?
) -> NSLinguisticTag?
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Parameters 

`string`  

The position of the initial character.

`charIndex`  

The linguistic unit. See NSLinguisticTaggerUnit for possible values.

`unit`  

The tag scheme. See NSLinguisticTagScheme for possible values.

`scheme`  

A pointer to the token range.

## Return Value

Returns the tag for the requested tag scheme and linguistic unit, or `nil`. If a tag is returned, this function returns by reference the range of the token to `tokenRange`.

## Discussion

This is a convenience method for initializing a linguistic tagger, setting the string property, and calling the tag(for:at:unit:scheme:orthography:tokenRange:) method. If you analyze the same string more than once, you should create a linguistic tagger object instead of calling this method.

## See Also

### Getting Linguistic Tags

func tag(at: Int, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, tokenRange: NSRangePointer?) -> NSLinguisticTag?

Returns a tag for a single scheme, for a given linguistic unit, at the specified character position.

Deprecated

func tag(at: Int, scheme: NSLinguisticTagScheme, tokenRange: NSRangePointer?, sentenceRange: NSRangePointer?) -> NSLinguisticTag?

Returns a tag for a single scheme at the specified character position.

Deprecated

func tags(in: NSRange, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, tokenRanges: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> [NSLinguisticTag]

Returns an array of linguistic tags and token ranges for a given string range and linguistic unit.

Deprecated

func tags(in: NSRange, scheme: String, options: NSLinguisticTagger.Options, tokenRanges: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> [String]

Returns an array of linguistic tags and token ranges for a given string range.

Deprecated

class func tags(for: String, range: NSRange, unit: NSLinguisticTaggerUnit, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, orthography: NSOrthography?, tokenRanges: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> [NSLinguisticTag]

Returns an array of linguistic tags and token ranges for a given string and linguistic unit.

Deprecated

