

- Foundation
- NSSpellServer
-  isWord(inUserDictionaries:caseSensitive:) 

Instance Method

# isWord(inUserDictionaries:caseSensitive:)

Indicates whether a given word is in the user’s list of learned words or the document’s list of words to ignore.

Mac Catalyst 13.0+macOS 10.0+

``` source
func isWord(
    inUserDictionaries word: String,
    caseSensitive flag: Bool
) -> Bool
```

## Parameters 

`word`  

The word to compare with those in the user dictionaries.

`flag`  

Specifies whether the comparison is case sensitive.

## Return Value

A Boolean value indicating whether the word is in the user dictionaries. If true, the word is acceptable to the user.

