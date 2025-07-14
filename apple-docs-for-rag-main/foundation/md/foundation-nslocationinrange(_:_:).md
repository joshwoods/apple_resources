

- Foundation
-  NSLocationInRange(\_:\_:) 

Function

# NSLocationInRange(\_:\_:)

Returns a Boolean value that indicates whether a specified position is in a given range.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSLocationInRange(
    _ loc: Int,
    _ range: NSRange
) -> Bool
```

## Return Value

true if `loc` lies within `range`—that is, if it’s greater than or equal to `range.location` and less than `range.location` plus `range.length`.

## See Also

### Managing ranges

func NSEqualRanges(NSRange, NSRange) -> Bool

Returns a Boolean value that indicates whether two given ranges are equal.

func NSIntersectionRange(NSRange, NSRange) -> NSRange

Returns the intersection of the specified ranges.

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

