

- Foundation
- NSString
-  enumerateLinguisticTags(in:scheme:options:orthography:using:) Deprecated

Instance Method

# enumerateLinguisticTags(in:scheme:options:orthography:using:)

Performs linguistic analysis on the specified string by enumerating the specific range of the string, providing the Block with the located tags.

iOS 5.0–18.4DeprecatediPadOS 5.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.7–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func enumerateLinguisticTags(
    in range: NSRange,
    scheme: NSLinguisticTagScheme,
    options: NSLinguisticTagger.Options = [],
    orthography: NSOrthography?,
    using block: (NSLinguisticTag?, NSRange, NSRange, UnsafeMutablePointer) -> Void
)
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Parameters 

`range`  

The range of the string to analyze.

`scheme`  

The tag scheme to use. See Linguistic Tag Schemes for supported values.

`options`  

The linguistic tagger options to use. See NSLinguisticTagger.Optionsfor the constants. These constants can be combined using the C-Bitwise OR operator.

`orthography`  

The orthography of the string. If `nil`, the linguistic tagger will attempt to determine the orthography from the string content.

`block`  

The Block to apply to the string.

The block takes four arguments:

tag  
The tag scheme for the token. The opts parameter specifies the types of tagger options that are located.

tokenRange  
The range of a string matching the tag scheme.

sentenceRange  
The range of the sentence in which the token is found.

stop  
A reference to a Boolean value. The block can set the value to true to stop further processing of the array. The `stop` argument is an out-only argument. You should only ever set this Boolean to true within the Block.

## Discussion

This is a convenience method. It is the equivalent of creating an instance of `NSLinguisticTagger`, specifying the receiver as the string to be analyzed, and the orthography (or `nil`) and then invoking the NSLinguisticTagger method or enumerateTags(in:scheme:options:using:).

## See Also

### Performing Linguistic Analysis

func linguisticTags(in: NSRange, scheme: NSLinguisticTagScheme, options: NSLinguisticTagger.Options, orthography: NSOrthography?, tokenRanges: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> [NSLinguisticTag]

Returns an array of linguistic tags for the specified range and requested tags within the receiving string.

Deprecated

struct EnumerationOptions

Constants to specify kinds of substrings and styles of enumeration.

