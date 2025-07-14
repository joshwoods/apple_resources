

- UIKit
- UITextChecker
-  rangeOfMisspelledWord(in:range:startingAt:wrap:language:) 

Instance Method

# rangeOfMisspelledWord(in:range:startingAt:wrap:language:)

Initiates a search of a range of a string for a misspelled word.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func rangeOfMisspelledWord(
    in stringToCheck: String,
    range: NSRange,
    startingAt startingOffset: Int,
    wrap wrapFlag: Bool,
    language: String
) -> NSRange
```

## Parameters 

`stringToCheck`  

The string to check for misspelled words.

`range`  

The range of `stringToCheck` to check for a misspelled word.

`startingOffset`  

The offset within `range` of `stringToCheck` to begin checking for misspelled words.

`wrapFlag`  

true to continue checking from the beginning of `range` if no misspelled word is found between `startingOffset` and the end of `range`. Specify false to have spell-checking end at the end of `range`.

`language`  

The language of the of words to be checked for correct spelling. This string is a ISO 639-1 language code or a combined ISO 639-1 language code and ISO 3166-1 regional code (for example, `fr_FR`).

## Return Value

The range of the first misspelled word encountered or `{NSNotFound, 0}` if none is found.

## Discussion

To search an entire string or a range within that string, call this method in a loop, resetting `startingOffset` from each returned range, until you reach the end of the string or specified range within the string.

