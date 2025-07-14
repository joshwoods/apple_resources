

- Swift Testing
- Tag
-  ..\

Operator

# ..\

Returns a partial range up to, but not including, its upper bound.

Swift TestingSwiftiOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
static func .. PartialRangeUpTo
```

## Parameters 

`maximum`  

The upper bound for the range.

## Discussion

Use the prefix half-open range operator (prefix `..` instance that includes any value less than `5.0`.

```
let upToFive = ..

You can use this type of partial range of a collection’s indices to represent the range from the start of the collection up to, but not including, the partial range’s upper bound.

```
let numbers = [10, 20, 30, 40, 50, 60, 70]
print(numbers[..

Precondition

`maximum` must compare equal to itself (i.e. cannot be NaN).

