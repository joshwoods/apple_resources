

- Swift
- Int8
-  quotientAndRemainder(dividingBy:) 

Instance Method

# quotientAndRemainder(dividingBy:)

Returns the quotient and remainder of this value divided by the given value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func quotientAndRemainder(dividingBy rhs: Self) -> (quotient: Self, remainder: Self)
```

## Parameters 

`rhs`  

The value to divide this value by.

## Return Value

A tuple containing the quotient and remainder of this value divided by `rhs`. The remainder has the same sign as `lhs`.

## Discussion

Use this method to calculate the quotient and remainder of a division at the same time.

```
let x = 1_000_000
let (q, r) = x.quotientAndRemainder(dividingBy: 933)
// q == 1071
// r == 757
```

