

- Foundation
-  NSRange 

Type Alias

# NSRange

A structure used to describe a portion of a series, such as characters in a string or objects in an array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias NSRange = _NSRange
```

## Discussion

Foundation functions that operate on ranges include the following:

- NSEqualRanges(_:_:)

- NSIntersectionRange(_:_:)

- NSLocationInRange(_:_:)

- NSMakeRange(_:_:)

- NSMaxRange(_:)

- NSRangeFromString(_:)

- NSStringFromRange(_:)

- NSUnionRange(_:_:)

## Topics

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

func NSUnionRange(NSRange, NSRange) -> NSRange

Returns the union of the specified ranges.

### Related types

typealias NSRangePointer

Type indicating a parameter is a pointer to an `NSRange` structure.

let NSNotFound: Int

A value indicating that a requested item couldn’t be found or doesn’t exist.

