

- Foundation
- NSTextCheckingResult
-  grammarCheckingResult(range:details:) 

Type Method

# grammarCheckingResult(range:details:)

Creates and returns a text checking result with the specified array of grammatical errors.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func grammarCheckingResult(
    range: NSRange,
    details: [[String : Any]]
) -> NSTextCheckingResult
```

## Parameters 

`range`  

The range of the detected result.

`details`  

An array of details regarding the grammatical errors. This array of strings is suitable for presenting to the user.

## Return Value

Returns an `NSTextCheckingResult` with the specified range and a resultType of grammar.

## See Also

### Text Checking Results for Grammar

var grammarDetails: [[String : Any]]?

The details of a located grammatical type checking result.

