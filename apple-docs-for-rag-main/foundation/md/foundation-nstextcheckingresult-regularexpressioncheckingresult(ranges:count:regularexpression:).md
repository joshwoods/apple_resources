

- Foundation
- NSTextCheckingResult
-  regularExpressionCheckingResult(ranges:count:regularExpression:) 

Type Method

# regularExpressionCheckingResult(ranges:count:regularExpression:)

Creates and returns a type checking result with the specified regular expression data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func regularExpressionCheckingResult(
    ranges: NSRangePointer,
    count: Int,
    regularExpression: NSRegularExpression
) -> NSTextCheckingResult
```

## Parameters 

`ranges`  

A C array of ranges, which must have at least one element, and the first element represents the overall range.

`count`  

The number of items in the `ranges` array.

`regularExpression`  

The regular expression.

## Return Value

Returns an `NSTextCheckingResult` with the specified range and a resultType of regularExpression.

## See Also

### Text Checking Results for Regular Expressions

var regularExpression: NSRegularExpression?

The regular expression of a type checking result.

