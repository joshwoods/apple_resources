

- Foundation
- NSTextCheckingResult
-  numberOfRanges 

Instance Property

# numberOfRanges

Returns the number of ranges.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var numberOfRanges: Int { get }
```

## Discussion

A result must have at least one range, but may optionally have more (for example, to represent regular expression capture groups).

Passing range(at:) the value `0` always returns the value of the the range property. Additional ranges, if any, will have indexes from `1` to ``` numberOfRanges``-1 ```.

## See Also

### Text Checking Type Range and Type

var range: NSRange

Returns the range of the result that the receiver represents.

var resultType: NSTextCheckingResult.CheckingType

Returns the text checking result type that the receiver represents.

func range(at: Int) -> NSRange

Returns the result type that the range represents.

