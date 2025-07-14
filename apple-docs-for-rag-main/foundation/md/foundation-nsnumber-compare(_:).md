

- Foundation
- NSNumber
-  compare(\_:) 

Instance Method

# compare(\_:)

Returns an `NSComparisonResult` value that indicates whether the number object’s value is greater than, equal to, or less than a given number.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func compare(_ otherNumber: NSNumber) -> ComparisonResult
```

## Parameters 

`otherNumber`  

The number to compare to the number object’s value.

This value must not be `nil`. If the value is `nil`, the behavior is undefined and may change in future versions of macOS.

## Return Value

`NSOrderedAscending` if the value of `otherNumber` is greater than the number object’s, `NSOrderedSame` if they’re equal, and `NSOrderedDescending` if the value of `otherNumber` is less than the number object’s.

## Discussion

The compare(_:) method follows the standard C rules for type conversion. For example, if you compare an `NSNumber` object that has an integer value with an `NSNumber` object that has a floating point value, the integer value is converted to a floating-point value for comparison.

## See Also

### Comparing NSNumber Objects

func isEqual(to: NSNumber) -> Bool

Returns a Boolean value that indicates whether the number object’s value and a given number are equal.

