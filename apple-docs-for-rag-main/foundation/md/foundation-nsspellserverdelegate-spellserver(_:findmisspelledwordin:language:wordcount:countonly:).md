

- Foundation
- NSSpellServerDelegate
-  spellServer(\_:findMisspelledWordIn:language:wordCount:countOnly:) 

Instance Method

# spellServer(\_:findMisspelledWordIn:language:wordCount:countOnly:)

Asks the delegate to search for a misspelled word in a given string, using the specified language, and marking the first misspelled word found by returning its range within the string.

Mac Catalyst 13.0+macOS 10.0+

``` source
optional func spellServer(
    _ sender: NSSpellServer,
    findMisspelledWordIn stringToCheck: String,
    language: String,
    wordCount: UnsafeMutablePointer,
    countOnly: Bool
) -> NSRange
```

## Parameters 

`sender`  

The `NSSpellServer` object that sent this message.

`stringToCheck`  

The string to search for the misspelled word.

`language`  

The language to use for the search.

`wordCount`  

On output, returns by reference the number of words from the beginning of the string object until the misspelled word (or the end of string).

`countOnly`  

If true, the method only counts the words in the string object and does not spell checking.

## Return Value

The range of the misspelled word within the given string.

## Discussion

Send isWord(inUserDictionaries:caseSensitive:) to the spelling server to determine if the word exists in the user’s language dictionaries.

## See Also

### Check Grammar and Spelling in Strings

func spellServer(NSSpellServer, check: String, offset: Int, types: NSTextCheckingTypes, options: [String : Any]?, orthography: NSOrthography?, wordCount: UnsafeMutablePointer&lt;Int>) -> [NSTextCheckingResult]?

Gives the delegate the opportunity to analyze both the spelling and grammar simultaneously, which is more efficient.

func spellServer(NSSpellServer, suggestGuessesForWord: String, inLanguage: String) -> [String]?

Gives the delegate the opportunity to suggest guesses to the sender for the correct spelling of the given misspelled word in the specified language.

func spellServer(NSSpellServer, checkGrammarIn: String, language: String?, details: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> NSRange

Gives the delegate the opportunity to customize the grammatical analysis of a given string.

