

- Foundation
- NSTextCheckingResult
-  replacementCheckingResult(range:replacementString:) 

Type Method

# replacementCheckingResult(range:replacementString:)

Creates and returns a text checking result with the specified replacement string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func replacementCheckingResult(
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

Returns an `NSTextCheckingResult` with the specified range and a resultType of replacement.

## See Also

### Text Checking Results for Text Replacement

var replacementString: String?

A replacement string from one of a number of replacement checking results.

