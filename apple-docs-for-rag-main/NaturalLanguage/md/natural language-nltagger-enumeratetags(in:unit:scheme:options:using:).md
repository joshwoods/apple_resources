

- Natural Language
- NLTagger
-  enumerateTags(in:unit:scheme:options:using:) 

Instance Method

# enumerateTags(in:unit:scheme:options:using:)

Enumerates a block over the tagger’s string, given a range, token unit, and tag scheme.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@nonobjc
func enumerateTags(
    in range: Range,
    unit: NLTokenUnit,
    scheme: NLTagScheme,
    options: NLTagger.Options = [],
    using block: (NLTag?, Range) -> Bool
)
```

## Parameters 

`range`  

The range of the string you want the tagger to analyze.

`unit`  

The linguistic unit of scale you’re interested in, such as NLTokenUnit.word, NLTokenUnit.sentence, NLTokenUnit.paragraph, or NLTokenUnit.document.

`scheme`  

The tag scheme the tagger uses to tag the string, such as language or script. This scheme determines which types of NLTag the method passes to your block. For other tag schemes, see NLTagScheme.

`options`  

The set of linguistic tagger options to use, such as omitWhitespace. For all available options, see NLTagger.Options.

`block`  

The block this method uses to iterate over the tagger’s string property. The block has the following parameters:

tag  
The tag of the token.

tokenRange  
The range of the token.

stop  
A reference to a Boolean value. The block can set the value to `true` to stop further processing of the set. The `stop` argument is an out-only argument. You should only ever set this Boolean to `true` within the block.

## Discussion

Use this method to iterate your block over the given range of a string. The method divides up the string with the given NLTokenUnit and NLTagScheme and then calls your block. For example, use the lexicalClass tag scheme to identify which tokens are parts of speech, types of whitespace, or types of punctuation. Use the lemma tag scheme to identify the stem form of each word token, if known.

Important

This method enumerates over the ranges of all tokens that intersect the specified range.

## See Also

### Enumerating linguistic tags

struct Options

Constants for linguistic tagger enumeration specifying which tokens to omit and whether to join names.

struct NLTag

A token type, lexical class, name, lemma, language, or script returned by a linguistic tagger for natural language text.

