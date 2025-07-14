

- Foundation
- NSSpellServerDelegate
-  spellServer(\_:suggestGuessesForWord:inLanguage:) 

Instance Method

# spellServer(\_:suggestGuessesForWord:inLanguage:)

Gives the delegate the opportunity to suggest guesses to the sender for the correct spelling of the given misspelled word in the specified language.

Mac Catalyst 13.0+macOS 10.0+

``` source
optional func spellServer(
    _ sender: NSSpellServer,
    suggestGuessesForWord word: String,
    inLanguage language: String
) -> [String]?
```

## Parameters 

`sender`  

The `NSSpellServer` object that sent this message.

`word`  

The misspelled word.

`language`  

The language to use for the guesses.

## Return Value

An array of `NSString` objects indicating possible correct spellings.

## See Also

### Check Grammar and Spelling in Strings

func spellServer(NSSpellServer, check: String, offset: Int, types: NSTextCheckingTypes, options: [String : Any]?, orthography: NSOrthography?, wordCount: UnsafeMutablePointer&lt;Int>) -> [NSTextCheckingResult]?

Gives the delegate the opportunity to analyze both the spelling and grammar simultaneously, which is more efficient.

func spellServer(NSSpellServer, checkGrammarIn: String, language: String?, details: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> NSRange

Gives the delegate the opportunity to customize the grammatical analysis of a given string.

func spellServer(NSSpellServer, findMisspelledWordIn: String, language: String, wordCount: UnsafeMutablePointer&lt;Int>, countOnly: Bool) -> NSRange

Asks the delegate to search for a misspelled word in a given string, using the specified language, and marking the first misspelled word found by returning its range within the string.

