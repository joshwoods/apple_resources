

- Foundation
- NSSpellServerDelegate
-  spellServer(\_:checkGrammarIn:language:details:) 

Instance Method

# spellServer(\_:checkGrammarIn:language:details:)

Gives the delegate the opportunity to customize the grammatical analysis of a given string.

macOS 10.5+

``` source
optional func spellServer(
    _ sender: NSSpellServer,
    checkGrammarIn stringToCheck: String,
    language: String?,
    details: AutoreleasingUnsafeMutablePointer?
) -> NSRange
```

## Parameters 

`sender`  

Spell server satisfying a grammatical analysis request.

`stringToCheck`  

String to analyze.

`language`  

Language use in `string`. When `nil`, the language selected in the Spelling panel is used.

`details`  

On output, dictionaries describing grammar-analysis details within the flagged grammatical unit. See the NSSpellServer class for information about these dictionaries.

## Return Value

Location of the first flagged grammatical unit within `string`.

## See Also

### Check Grammar and Spelling in Strings

func spellServer(NSSpellServer, check: String, offset: Int, types: NSTextCheckingTypes, options: [String : Any]?, orthography: NSOrthography?, wordCount: UnsafeMutablePointer&lt;Int>) -> [NSTextCheckingResult]?

Gives the delegate the opportunity to analyze both the spelling and grammar simultaneously, which is more efficient.

func spellServer(NSSpellServer, suggestGuessesForWord: String, inLanguage: String) -> [String]?

Gives the delegate the opportunity to suggest guesses to the sender for the correct spelling of the given misspelled word in the specified language.

func spellServer(NSSpellServer, findMisspelledWordIn: String, language: String, wordCount: UnsafeMutablePointer&lt;Int>, countOnly: Bool) -> NSRange

Asks the delegate to search for a misspelled word in a given string, using the specified language, and marking the first misspelled word found by returning its range within the string.

