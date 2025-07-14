

- Swift
- UInt64
-  -(\_:\_:) 

Operator

# -(\_:\_:)

Subtracts one value from another and produces their difference.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func - (lhs: UInt64, rhs: UInt64) -> UInt64
```

## Parameters 

`lhs`  

A numeric value.

`rhs`  

The value to subtract from `lhs`.

## Discussion

The subtraction operator (`-`) calculates the difference of its two arguments. For example:

```
8 - 3                   // 5
-10 - 5                 // -15
100 - -5                // 105
10.5 - 100.0            // -89.5
```

You cannot use `-` with arguments of different types. To subtract values of different types, convert one of the values to the other value’s type.

```
let x: UInt8 = 21
let y: UInt = 1000000
y - UInt(x)             // 999979
```

The difference of the two arguments must be representable in the arguments’ type. In the following example, the result of `21 - 50` is less than zero, the minimum representable `UInt8` value:

```
x - 50                  // Overflow error
```

Note

Overflow checking is not performed in `-Ounchecked` builds.

If you want to opt out of overflow checking and wrap the result in case of any overflow, use the overflow subtraction operator (`&-`).

```
x &- 50                 // 227
```

