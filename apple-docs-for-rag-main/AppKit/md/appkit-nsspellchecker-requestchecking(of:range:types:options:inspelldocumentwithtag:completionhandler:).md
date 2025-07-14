

- AppKit
- NSSpellChecker
-  requestChecking(of:range:types:options:inSpellDocumentWithTag:completionHandler:) 

Instance Method

# requestChecking(of:range:types:options:inSpellDocumentWithTag:completionHandler:)

Requests that the string be checked in the background.

macOS 10.6+

``` source
func requestChecking(
    of stringToCheck: String,
    range: NSRange,
    types checkingTypes: NSTextCheckingTypes,
    options: [NSSpellChecker.OptionKey : Any]? = nil,
    inSpellDocumentWithTag tag: Int,
    completionHandler: ((Int, [NSTextCheckingResult], NSOrthography, Int) -> Void)? = nil
) -> Int
```

## Parameters 

`stringToCheck`  

The string to check.

`range`  

The range of the string to check.

`checkingTypes`  

The type of checking to be performed. The possible constants are listed in NSTextCheckingResult.CheckingType and can be combined using the C bit-wise `OR` operator to perform multiple checks at the same time.

`options`  

The options dictionary specifying the types of checking to perform. See NSSpellChecker.OptionKey for the possible keys and expected values.

`tag`  

An identifier unique within the application used to inform the spell checker which document that text is associated, potentially for many purposes, not necessarily just for ignored words. A value of 0 can be passed in for text not associated with a particular document.

`completionHandler`  

The completion handler block object will be called (in an arbitrary context) when results are available, with the sequence number and results.

The block takes four arguments:

sequenceNumber  
A monotonically increasing sequence number.

results  
An array of NSTextCheckingResult objects describing particular items found during checking and their individual ranges, sorted by range origin, then range end, then result type.

orthography  
The orthography of the string.

wordCount  
The number of words in the range of the string.

## Return Value

The return value is a monotonically increasing sequence number that can be used to keep track of requests in flight.

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

func guesses(forWordRange: NSRange, in: String, language: String?, inSpellDocumentWithTag: Int) -> [String]?

Returns an array of possible substitutions for the specified string.

