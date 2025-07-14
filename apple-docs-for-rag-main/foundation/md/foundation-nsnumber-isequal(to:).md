

- Foundation
- NSNumber
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Returns a Boolean value that indicates whether the number object’s value and a given number are equal.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isEqual(to number: NSNumber) -> Bool
```

## Parameters 

`number`  

The number to compare to the number object’s value.

## Return Value

true if the number object’s value and `number` are equal, otherwise false.

## Discussion

Two `NSNumber` objects are considered equal if they have the same id values or if they have equivalent values (as determined by the compare(_:) method).

This method is more efficient than compare(_:) if you know the two objects are numbers.

## See Also

### Comparing NSNumber Objects

func compare(NSNumber) -> ComparisonResult

Returns an `NSComparisonResult` value that indicates whether the number object’s value is greater than, equal to, or less than a given number.

