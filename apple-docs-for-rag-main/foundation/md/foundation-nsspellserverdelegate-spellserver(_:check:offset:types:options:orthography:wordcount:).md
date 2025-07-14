

- Foundation
- NSSpellServerDelegate
-  spellServer(\_:check:offset:types:options:orthography:wordCount:) 

Instance Method

# spellServer(\_:check:offset:types:options:orthography:wordCount:)

Gives the delegate the opportunity to analyze both the spelling and grammar simultaneously, which is more efficient.

macOS 10.6+

``` source
optional func spellServer(
    _ sender: NSSpellServer,
    check stringToCheck: String,
    offset: Int,
    types checkingTypes: NSTextCheckingTypes,
    options: [String : Any]? = nil,
    orthography: NSOrthography?,
    wordCount: UnsafeMutablePointer
) -> [NSTextCheckingResult]?
```

## Parameters 

`sender`  

Spell server making the analysis request.

`stringToCheck`  

String to analyze.

`offset`  

The offset in the string.

`checkingTypes`  

The text checking types to perform.

`options`  

A dictionary defining the actions to be taken while checking this string. See Constants in NSSpellChecker for the possible keys.

`orthography`  

The identified orthography of `stringToCheck`. See NSOrthography for more information.

`wordCount`  

On output, returns by-reference the number of words from the beginning of the string object until the misspelled word (or the end of string).

## Return Value

An array of NSTextCheckingResult instances of the spelling, grammar, or correction types, depending on the `checkingTypes` requested.

## Discussion

This method is optional, but if implemented it will be called during the course of unified text checking via the `NSSpellChecker` checkSpelling(of:startingAt:) and requestChecking(of:range:types:options:inSpellDocumentWithTag:completionHandler:) methods. This allows spelling and grammar checking to be performed simultaneously, which can be significantly more efficient, and allows the delegate to return autocorrection results as well.

If this method is not implemented, then unified text checking will call the separate spelling and grammar checking methods instead.

This method may be called repeatedly with strings representing different subranges of the string that was originally requested to be checked; the offset argument represents the offset of the portion passed in to this method within that original string, and should be added to the origin of the range in any NSTextCheckingResult returned.

## See Also

### Related Documentation

Spell Checking Programming Topics

### Check Grammar and Spelling in Strings

func spellServer(NSSpellServer, suggestGuessesForWord: String, inLanguage: String) -> [String]?

Gives the delegate the opportunity to suggest guesses to the sender for the correct spelling of the given misspelled word in the specified language.

func spellServer(NSSpellServer, checkGrammarIn: String, language: String?, details: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> NSRange

Gives the delegate the opportunity to customize the grammatical analysis of a given string.

func spellServer(NSSpellServer, findMisspelledWordIn: String, language: String, wordCount: UnsafeMutablePointer&lt;Int>, countOnly: Bool) -> NSRange

Asks the delegate to search for a misspelled word in a given string, using the specified language, and marking the first misspelled word found by returning its range within the string.

