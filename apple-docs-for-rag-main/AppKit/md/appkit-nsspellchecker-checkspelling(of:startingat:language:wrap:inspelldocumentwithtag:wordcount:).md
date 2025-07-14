

- AppKit
- NSSpellChecker
-  checkSpelling(of:startingAt:language:wrap:inSpellDocumentWithTag:wordCount:) 

Instance Method

# checkSpelling(of:startingAt:language:wrap:inSpellDocumentWithTag:wordCount:)

Starts the search for a misspelled word in a string starting at specified offset within the string.

macOS

``` source
func checkSpelling(
    of stringToCheck: String,
    startingAt startingOffset: Int,
    language: String?,
    wrap wrapFlag: Bool,
    inSpellDocumentWithTag tag: Int,
    wordCount: UnsafeMutablePointer?
) -> NSRange
```

## Parameters 

`stringToCheck`  

The string object containing the words to spellcheck.

`startingOffset`  

The offset within `stringToCheck` at which to begin spellchecking.

`language`  

The language of the words in the string. If `language` is `nil`, or if you obtain the value by sending language() to `self`, the current selection in the Spelling panel’s pop-up menu is used. Do not pass in an empty string for `language`.

`wrapFlag`  

true to indicate that spell checking should continue at the beginning of the string when the end of the string is reached; false to indicate that spellchecking should stop at the end of the document.

`tag`  

An identifier unique within the application used to inform the spell checker which document that text is associated, potentially for many purposes, not necessarily just for ignored words. A value of 0 can be passed in for text not associated with a particular document.

`wordCount`  

Returns by indirection a count of the words spell-checked up to and including the first error (if any), or -1 if the spell checker fails or does not support word counting. Specify `NULL` if you do not want this word count.

## Return Value

The range of the first misspelled word and optionally (and by reference) the count of words spellchecked in the string in `wordCount`.

## See Also

### Checking Strings for Spelling and Grammar

func countWords(in: String, language: String?) -> Int

Returns the number of words in the specified string.

func checkSpelling(of: String, startingAt: Int) -> NSRange

Starts the search for a misspelled word in `stringToCheck` starting at `startingOffset` within the string object.

func checkGrammar(of: String, startingAt: Int, language: String?, wrap: Bool, inSpellDocumentWithTag: Int, details: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> NSRange

Initiates a grammatical analysis of a given string.

func check(String, range: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any]?, inSpellDocumentWithTag: Int, orthography: AutoreleasingUnsafeMutablePointer&lt;NSOrthography?>?, wordCount: UnsafeMutablePointer&lt;Int>?) -> [NSTextCheckingResult]

Requests unified text checking for the given range of the given string.

func requestChecking(of: String, range: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any]?, inSpellDocumentWithTag: Int, completionHandler: ((Int, [NSTextCheckingResult], NSOrthography, Int) -> Void)?) -> Int

Requests that the string be checked in the background.

func guesses(forWordRange: NSRange, in: String, language: String?, inSpellDocumentWithTag: Int) -> [String]?

Returns an array of possible substitutions for the specified string.

