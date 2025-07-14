

- Foundation
- NSTextCheckingResult
-  grammarDetails 

Instance Property

# grammarDetails

The details of a located grammatical type checking result.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var grammarDetails: [[String : Any]]? { get }
```

## Discussion

This array of strings is suitable for presenting to the user.

## See Also

### Text Checking Results for Grammar

class func grammarCheckingResult(range: NSRange, details: [[String : Any]]) -> NSTextCheckingResult

Creates and returns a text checking result with the specified array of grammatical errors.

