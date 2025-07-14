

- Foundation
-  NSUnionRange(\_:\_:) 

Function

# NSUnionRange(\_:\_:)

Returns the union of the specified ranges.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSUnionRange(
    _ range1: NSRange,
    _ range2: NSRange
) -> NSRange
```

## Return Value

A range covering all indices in and between `range1` and `range2`. If one range is completely contained in the other, the returned range is equal to the larger range.

## See Also

### Managing ranges

func NSEqualRanges(NSRange, NSRange) -> Bool

Returns a Boolean value that indicates whether two given ranges are equal.

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

