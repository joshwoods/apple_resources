

- AppKit
- NSSpellChecker
-  guesses(forWordRange:in:language:inSpellDocumentWithTag:) 

Instance Method

# guesses(forWordRange:in:language:inSpellDocumentWithTag:)

Returns an array of possible substitutions for the specified string.

macOS 10.6+

``` source
func guesses(
    forWordRange range: NSRange,
    in string: String,
    language: String?,
    inSpellDocumentWithTag tag: Int
) -> [String]?
```

## Parameters 

`range`  

The range of the string to check.

`string`  

The string to guess.

`language`  

The language of the string.

`tag`  

An identifier unique within the application used to inform the spell checker which document that text is associated, potentially for many purposes, not necessarily just for ignored words. A value of 0 can be passed in for text not associated with a particular document.

## Return Value

An array of strings containing possible replacement words.

## See Also

### Checking Strings for Spelling and Grammar

func countWords(in: String, language: String?) -> Int

Returns the number of words in the specified string.

func checkSpelling(of: String, startingAt: Int) -> NSRange

Starts the search for a misspelled word in `stringToCheck` starting at `startingOffset` within the string object.

func checkSpelling(of: String, startingAt: Int, language: String?, wrap: Bool, inSpellDocumentWithTag: Int, wordCount: UnsafeMutablePointer&lt;Int>?) -> NSRange

Starts the search for a misspelled word in a string starting at specified offset within the string.

func checkGrammar(of: String, startingAt: Int, language: String?, wrap: Bool, inSpellDocumentWithTag: Int, details: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> NSRange

Initiates a grammatical analysis of a given string.

func check(String, range: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any]?, inSpellDocumentWithTag: Int, orthography: AutoreleasingUnsafeMutablePointer&lt;NSOrthography?>?, wordCount: UnsafeMutablePointer&lt;Int>?) -> [NSTextCheckingResult]

Requests unified text checking for the given range of the given string.

func requestChecking(of: String, range: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any]?, inSpellDocumentWithTag: Int, completionHandler: ((Int, [NSTextCheckingResult], NSOrthography, Int) -> Void)?) -> Int

Requests that the string be checked in the background.

