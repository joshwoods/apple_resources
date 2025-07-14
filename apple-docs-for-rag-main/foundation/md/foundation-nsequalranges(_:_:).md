

- Foundation
-  NSEqualRanges(\_:\_:) 

Function

# NSEqualRanges(\_:\_:)

Returns a Boolean value that indicates whether two given ranges are equal.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSEqualRanges(
    _ range1: NSRange,
    _ range2: NSRange
) -> Bool
```

## Return Value

true if `range1` and `range2` have the same locations and lengths.

## See Also

### Managing ranges

func NSIntersectionRange(NSRange, NSRange) -> NSRange

Returns the intersection of the specified ranges.

func NSLocationInRange(Int, NSRange) -> Bool

Returns a Boolean value that indicates whether a specified position is in a given range.

func NSMakeRange(Int, Int) -> NSRange

Creates a new NSRange from the specified values.

func NSMaxRange(NSRange) -> Int

Returns the sum of the location and length of the range.

func NSRangeFromString(String) -> NSRange

Returns a range from a textual representation.

func NSStringFromRange(NSRange) -> String

Returns a string representation of a range.

func NSUnionRange(NSRange, NSRange) -> NSRange

Returns the union of the specified ranges.

