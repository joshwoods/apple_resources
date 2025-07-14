

- Foundation
- NSTextCheckingResult
-  regularExpression 

Instance Property

# regularExpression

The regular expression of a type checking result.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var regularExpression: NSRegularExpression? { get }
```

## See Also

### Text Checking Results for Regular Expressions

class func regularExpressionCheckingResult(ranges: NSRangePointer, count: Int, regularExpression: NSRegularExpression) -> NSTextCheckingResult

Creates and returns a type checking result with the specified regular expression data.

