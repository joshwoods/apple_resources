

- Natural Language
- NLTagger
-  setLanguage(\_:range:) 

Instance Method

# setLanguage(\_:range:)

Sets the language for a range of text within the tagger’s string.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@nonobjc
func setLanguage(
    _ language: NLLanguage,
    range: Range
)
```

## Parameters 

`language`  

The language of the text range.

`range`  

The range of the string that is being assigned a language.

## See Also

### Determining the dominant language and orthography

var dominantLanguage: NLLanguage?

The dominant language of the string set for the linguistic tagger.

func setOrthography(NSOrthography, range: Range&lt;String.Index>)

Sets the orthography for the specified range.

