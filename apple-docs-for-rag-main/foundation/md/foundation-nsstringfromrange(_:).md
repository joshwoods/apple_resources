

- Foundation
-  NSStringFromRange(\_:) 

Function

# NSStringFromRange(\_:)

Returns a string representation of a range.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSStringFromRange(_ range: NSRange) -> String
```

## Return Value

A string of the form “{a, b}”, where a and b are non-negative integers representing `aRange`.

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

func NSUnionRange(NSRange, NSRange) -> NSRange

Returns the union of the specified ranges.

