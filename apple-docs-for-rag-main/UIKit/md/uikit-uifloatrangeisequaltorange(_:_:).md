

- UIKit
-  UIFloatRangeIsEqualToRange(\_:\_:) 

Function

# UIFloatRangeIsEqualToRange(\_:\_:)

Returns a Boolean indicating whether two float ranges are equivalent.

iOS 7.0–12.0DeprecatediPadOS 7.0–12.0DeprecatedMac CatalysttvOSvisionOSSwift 1.0–4.2Deprecated

``` source
func UIFloatRangeIsEqualToRange(
    _ range: UIFloatRange,
    _ otherRange: UIFloatRange
) -> Bool
```

## Parameters 

`range`  

The first range to compare.

`otherRange`  

The second range to compare.

## Discussion

Two ranges are considered equal when their minimum values are the same and their maximum values are the same. In practice, the minimum and maximum values do not have to be exactly equal, but the difference between each pair of values must be less than `FLT_EPSILON`.

## See Also

### Testing the range values

var isInfinite: Bool

Returns a Boolean indicating whether the specified float range is infinitely large.

