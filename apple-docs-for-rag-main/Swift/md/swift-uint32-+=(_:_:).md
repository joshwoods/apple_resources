

- Swift
- UInt32
-  +=(\_:\_:) 

Operator

# +=(\_:\_:)

Adds two values and stores the result in the left-hand-side variable.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func += (lhs: inout UInt32, rhs: UInt32)
```

## Parameters 

`lhs`  

The first value to add.

`rhs`  

The second value to add.

## Discussion

The sum of the two arguments must be representable in the arguments’ type. In the following example, the result of `21 + 120` is greater than the maximum representable `Int8` value:

```
var x: Int8 = 21
x += 120
// Overflow error
```

Note

Overflow checking is not performed in `-Ounchecked` builds.

