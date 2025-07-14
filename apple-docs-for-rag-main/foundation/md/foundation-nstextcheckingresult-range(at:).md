

- Foundation
- NSTextCheckingResult
-  range(at:) 

Instance Method

# range(at:)

Returns the result type that the range represents.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func range(at idx: Int) -> NSRange
```

## Parameters 

`idx`  

The index of the result.

## Return Value

The range of the result.

## Discussion

A result must have at least one range, but may optionally have more, for example, to represent regular expression capture groups.

Passing range(at:) the value `0` always returns the value of the range property. Additional ranges, if any, will have indexes from `1` to ``` numberOfRanges``-1 ```.

## See Also

### Text Checking Type Range and Type

var range: NSRange

Returns the range of the result that the receiver represents.

var resultType: NSTextCheckingResult.CheckingType

Returns the text checking result type that the receiver represents.

var numberOfRanges: Int

Returns the number of ranges.

