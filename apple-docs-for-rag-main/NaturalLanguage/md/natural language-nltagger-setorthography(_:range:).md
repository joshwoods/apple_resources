

- Natural Language
- NLTagger
-  setOrthography(\_:range:) 

Instance Method

# setOrthography(\_:range:)

Sets the orthography for the specified range.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@nonobjc
func setOrthography(
    _ orthography: NSOrthography,
    range: Range
)
```

## Parameters 

`orthography`  

The orthography for the given range.

`range`  

The range of the string that is being assigned an orthography.

## Discussion

If the orthography of the linguistic tagger is not set, it will determine it automatically from the contents of the text. You should call this method only if you know the orthography of the text by some other means.

## See Also

### Determining the dominant language and orthography

var dominantLanguage: NLLanguage?

The dominant language of the string set for the linguistic tagger.

func setLanguage(NLLanguage, range: Range&lt;String.Index>)

Sets the language for a range of text within the tagger’s string.

