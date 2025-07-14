

- Latent Semantic Mapping
-  LSMTextAddWords(\_:\_:\_:\_:) 

Function

# LSMTextAddWords(\_:\_:\_:\_:)

Breaks a string into words using the specified locale, and adds the words to the text.

Mac CatalystmacOS

``` source
func LSMTextAddWords(
    _ textref: LSMText,
    _ words: CFString,
    _ locale: CFLocale?,
    _ flags: CFOptionFlags
) -> OSStatus
```

## See Also

### Adding to the Text

func LSMTextAddToken(LSMText, CFData) -> OSStatus

Adds an arbitrary binary token to the text.

func LSMTextAddWord(LSMText, CFString) -> OSStatus

Adds a word to the text.

Parsing Flags

Options for parsing words to add to the text.

