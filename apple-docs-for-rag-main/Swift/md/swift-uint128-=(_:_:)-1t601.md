

- Swift
- UInt128
-  \>=(\_:\_:) 

Operator

# \>=(\_:\_:)

Returns a Boolean value indicating whether the value of the first argument is greater than or equal to that of the second argument.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func >= (lhs: Self, rhs: Other) -> Bool where Other : BinaryInteger
```

## Parameters 

`lhs`  

An integer to compare.

`rhs`  

Another integer to compare.

## Discussion

You can compare instances of any `BinaryInteger` types using the greater-than-or-equal-to operator (`>=`), even if the two instances are of different types.

