

- Foundation
- NSTextCheckingResult
-  correctionCheckingResult(range:replacementString:) 

Type Method

# correctionCheckingResult(range:replacementString:)

Creates and returns a text checking result after detecting a possible correction.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func correctionCheckingResult(
    range: NSRange,
    replacementString: String
) -> NSTextCheckingResult
```

## Parameters 

`range`  

The range of the detected result.

`replacementString`  

The suggested replacement string.

## Return Value

Returns an `NSTextCheckingResult` with the specified range and a resultType of spelling.

## See Also

### Related Documentation

var replacementString: String?

A replacement string from one of a number of replacement checking results.

### Text Checking Results for Spelling

class func spellCheckingResult(range: NSRange) -> NSTextCheckingResult

Creates and returns a text checking result with the range of a misspelled word.

