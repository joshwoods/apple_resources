

- AppKit
- NSSpellChecker
-  checkGrammar(of:startingAt:language:wrap:inSpellDocumentWithTag:details:) 

Instance Method

# checkGrammar(of:startingAt:language:wrap:inSpellDocumentWithTag:details:)

Initiates a grammatical analysis of a given string.

macOS 10.5+

``` source
func checkGrammar(
    of stringToCheck: String,
    startingAt startingOffset: Int,
    language: String?,
    wrap wrapFlag: Bool,
    inSpellDocumentWithTag tag: Int,
    details: AutoreleasingUnsafeMutablePointer?
) -> NSRange
```

## Parameters 

`stringToCheck`  

String to analyze.

`startingOffset`  

Location within `string` at which to start the analysis.

`language`  

Language use in `string`. When `nil`, the language selected in the Spelling panel is used.

`wrapFlag`  

true to specify that the analysis continue to the beginning of string when the end is reached.

false to have the analysis stop at the end of string.

`tag`  

An identifier unique within the application used to inform the spell checker which document that text is associated, potentially for many purposes, not necessarily just for ignored words. A value of 0 can be passed in for text not associated with a particular document.

`details`  

On output, dictionaries describing grammar-analysis details within the flagged grammatical unit. See the NSSpellServer class for information about these dictionaries.

## Return Value

Location of the first flagged grammatical unit.

## See Also

### Checking Strings for Spelling and Grammar

func countWords(in: String, language: String?) -> Int

Returns the number of words in the specified string.

func checkSpelling(of: String, startingAt: Int) -> NSRange

Starts the search for a misspelled word in `stringToCheck` starting at `startingOffset` within the string object.

func checkSpelling(of: String, startingAt: Int, language: String?, wrap: Bool, inSpellDocumentWithTag: Int, wordCount: UnsafeMutablePointer&lt;Int>?) -> NSRange

Starts the search for a misspelled word in a string starting at specified offset within the string.

func check(String, range: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any]?, inSpellDocumentWithTag: Int, orthography: AutoreleasingUnsafeMutablePointer&lt;NSOrthography?>?, wordCount: UnsafeMutablePointer&lt;Int>?) -> [NSTextCheckingResult]

Requests unified text checking for the given range of the given string.

func requestChecking(of: String, range: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any]?, inSpellDocumentWithTag: Int, completionHandler: ((Int, [NSTextCheckingResult], NSOrthography, Int) -> Void)?) -> Int

Requests that the string be checked in the background.

func guesses(forWordRange: NSRange, in: String, language: String?, inSpellDocumentWithTag: Int) -> [String]?

Returns an array of possible substitutions for the specified string.

