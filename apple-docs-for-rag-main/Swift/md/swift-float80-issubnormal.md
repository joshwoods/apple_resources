

- Swift
- Float80
-  isSubnormal 

Instance Property

# isSubnormal

A Boolean value indicating whether the instance is subnormal.

macOS 10.10+

``` source
var isSubnormal: Bool { get }
```

## Discussion

A *subnormal* value is a nonzero number that has a lesser magnitude than the smallest normal number. Subnormal values don’t use the full precision available to values of a type.

Zero is neither a normal nor a subnormal number. Subnormal numbers are often called *denormal* or *denormalized*—these are different names for the same concept.

