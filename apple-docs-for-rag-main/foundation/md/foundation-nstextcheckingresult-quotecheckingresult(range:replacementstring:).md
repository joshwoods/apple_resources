

- Foundation
- NSTextCheckingResult
-  quoteCheckingResult(range:replacementString:) 

Type Method

# quoteCheckingResult(range:replacementString:)

Creates and returns a text checking result with the specified quote-balanced replacement string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func quoteCheckingResult(
    range: NSRange,
    replacementString: String
) -> NSTextCheckingResult
```

## Parameters 

`range`  

The range of the detected result.

`replacementString`  

The replacement string.

## Return Value

Returns an `NSTextCheckingResult` with the specified range and a resultType of quote.

## See Also

### Text Checking Results for Typography

class func dashCheckingResult(range: NSRange, replacementString: String) -> NSTextCheckingResult

Creates and returns a text checking result with the specified dash corrected replacement string.

