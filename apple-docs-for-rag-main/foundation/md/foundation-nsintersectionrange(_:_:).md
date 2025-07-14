

- Foundation
-  NSIntersectionRange(\_:\_:) 

Function

# NSIntersectionRange(\_:\_:)

Returns the intersection of the specified ranges.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSIntersectionRange(
    _ range1: NSRange,
    _ range2: NSRange
) -> NSRange
```

## Return Value

A range describing the intersection of `range1` and `range2`—that is, a range containing the indices that exist in both ranges.

## Discussion

If the returned range’s length field is 0, then the two ranges don’t intersect, and the value of the location field is undefined.

## See Also

### Managing ranges

func NSEqualRanges(NSRange, NSRange) -> Bool

Returns a Boolean value that indicates whether two given ranges are equal.

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

