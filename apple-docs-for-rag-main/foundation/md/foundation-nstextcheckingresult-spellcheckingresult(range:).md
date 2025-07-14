

- Foundation
- NSTextCheckingResult
-  spellCheckingResult(range:) 

Type Method

# spellCheckingResult(range:)

Creates and returns a text checking result with the range of a misspelled word.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func spellCheckingResult(range: NSRange) -> NSTextCheckingResult
```

## Parameters 

`range`  

The range of the detected result.

## Return Value

Returns an `NSTextCheckingResult` with the specified range and a resultType of spelling.

## See Also

### Text Checking Results for Spelling

class func correctionCheckingResult(range: NSRange, replacementString: String) -> NSTextCheckingResult

Creates and returns a text checking result after detecting a possible correction.

