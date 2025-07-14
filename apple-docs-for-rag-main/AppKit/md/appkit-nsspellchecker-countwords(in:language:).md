

- AppKit
- NSSpellChecker
-  countWords(in:language:) 

Instance Method

# countWords(in:language:)

Returns the number of words in the specified string.

macOS

``` source
func countWords(
    in stringToCount: String,
    language: String?
) -> Int
```

## Parameters 

`stringToCount`  

The string to count the words in.

`language`  

The language of the string.

## Return Value

The number of words in the string or `-1` if word counting is unavailable or has not occurred for some reason.

## Discussion

If `language` is `nil`, the current selection in the Spelling panel’s pop-up menu is used.

## See Also

### Checking Strings for Spelling and Grammar

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

func guesses(forWordRange: NSRange, in: String, language: String?, inSpellDocumentWithTag: Int) -> [String]?

Returns an array of possible substitutions for the specified string.

