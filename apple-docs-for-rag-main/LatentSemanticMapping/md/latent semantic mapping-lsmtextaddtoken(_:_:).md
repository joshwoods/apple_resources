

- Latent Semantic Mapping
-  LSMTextAddToken(\_:\_:) 

Function

# LSMTextAddToken(\_:\_:)

Adds an arbitrary binary token to the text.

Mac CatalystmacOS

``` source
func LSMTextAddToken(
    _ textref: LSMText,
    _ token: CFData
) -> OSStatus
```

## Discussion

The order of tokens is significant if the map uses pairs or triplets, and the count of tokens is always significant.

## See Also

### Adding to the Text

func LSMTextAddWord(LSMText, CFString) -> OSStatus

Adds a word to the text.

func LSMTextAddWords(LSMText, CFString, CFLocale?, CFOptionFlags) -> OSStatus

Breaks a string into words using the specified locale, and adds the words to the text.

Parsing Flags

Options for parsing words to add to the text.

