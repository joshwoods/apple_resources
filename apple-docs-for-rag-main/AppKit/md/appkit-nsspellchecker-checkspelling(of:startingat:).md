

- AppKit
- NSSpellChecker
-  checkSpelling(of:startingAt:) 

Instance Method

# checkSpelling(of:startingAt:)

Starts the search for a misspelled word in `stringToCheck` starting at `startingOffset` within the string object.

macOS

``` source
func checkSpelling(
    of stringToCheck: String,
    startingAt startingOffset: Int
) -> NSRange
```

## Parameters 

`stringToCheck`  

The string to spell check.

`startingOffset`  

The offset at which to start checking.

## Return Value

Returns the range of the first misspelled word.

## Discussion

Wrapping occurs, but no ignored-words dictionary is used.

## See Also

### Checking Strings for Spelling and Grammar

func countWords(in: String, language: String?) -> Int

Returns the number of words in the specified string.

func checkSpelling(of: String, startingAt: Int, language: String?, wrap: Bool, inSpellDocumentWithTag: Int, wordCount: UnsafeMutablePointer&lt;Int>?) -> NSRange

Starts the search for a misspelled word in a string starting at specified offset within the string.

func checkGrammar(of: String, startingAt: Int, language: String?, wrap: Bool, inSpellDocumentWithTag: Int, details: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) -> NSRange

Initiates a grammatical analysis of a given string.

func check(String, range: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any]?, inSpellDocumentWithTag: Int, orthography: AutoreleasingUnsafeMutablePointer&lt;NSOrthography?>?, wordCount: UnsafeMutablePointer&lt;Int>?) -> [NSTextCheckingResult]

Requests unified text checking for the given range of the given string.

func requestChecking(of: String, range: NSRange, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any]?, inSpellDocumentWithTag: Int, completionHandler: ((Int, [NSTextCheckingResult], NSOrthography, Int) -> Void)?) -> Int

Requests that the string be checked in the background.

func guesses(forWordRange: NSRange, in: String, language: String?, inSpellDocumentWithTag: Int) -> [String]?

Returns an array of possible substitutions for the specified string.

