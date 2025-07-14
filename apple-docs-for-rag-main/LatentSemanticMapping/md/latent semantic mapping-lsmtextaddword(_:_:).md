

- Latent Semantic Mapping
-  LSMTextAddWord(\_:\_:) 

Function

# LSMTextAddWord(\_:\_:)

Adds a word to the text.

Mac CatalystmacOS

``` source
func LSMTextAddWord(
    _ textref: LSMText,
    _ word: CFString
) -> OSStatus
```

## Discussion

The order of words is significant if the map uses pairs or triplets, and the count of words is always significant.

## See Also

### Adding to the Text

func LSMTextAddToken(LSMText, CFData) -> OSStatus

Adds an arbitrary binary token to the text.

func LSMTextAddWords(LSMText, CFString, CFLocale?, CFOptionFlags) -> OSStatus

Breaks a string into words using the specified locale, and adds the words to the text.

Parsing Flags

Options for parsing words to add to the text.

