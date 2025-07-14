

- Foundation
- NSTextCheckingResult
-  resultType 

Instance Property

# resultType

Returns the text checking result type that the receiver represents.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var resultType: NSTextCheckingResult.CheckingType { get }
```

## Discussion

The possible result types for the built in checking capabilities are described in NSTextCheckingResult.CheckingType.

This property will be present for all returned `NSTextCheckingResult` instances.

## See Also

### Text Checking Type Range and Type

var range: NSRange

Returns the range of the result that the receiver represents.

var numberOfRanges: Int

Returns the number of ranges.

func range(at: Int) -> NSRange

Returns the result type that the range represents.

