

- Swift
- RangeSet
-  subtracting(\_:) 

Instance Method

# subtracting(\_:)

Returns a new set containing the contents of this range set that are not also in the given range set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func subtracting(_ other: RangeSet) -> RangeSet
```

Available when `Bound` conforms to `Comparable`.

## Parameters 

`other`  

The range set to subtract.

## Return Value

A new range set.

