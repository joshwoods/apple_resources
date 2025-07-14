

- Foundation
- NSTextCheckingResult
-  range 

Instance Property

# range

Returns the range of the result that the receiver represents.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var range: NSRange { get }
```

## Discussion

This property will be present for all returned `NSTextCheckingResult` instances.

## See Also

### Text Checking Type Range and Type

var resultType: NSTextCheckingResult.CheckingType

Returns the text checking result type that the receiver represents.

var numberOfRanges: Int

Returns the number of ranges.

func range(at: Int) -> NSRange

Returns the result type that the range represents.

