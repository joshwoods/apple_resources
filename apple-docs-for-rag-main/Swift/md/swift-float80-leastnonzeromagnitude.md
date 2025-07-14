

- Swift
- Float80
-  leastNonzeroMagnitude 

Type Property

# leastNonzeroMagnitude

The least positive number.

macOS 10.10+

``` source
static var leastNonzeroMagnitude: Float80 { get }
```

## Discussion

This value compares less than or equal to all positive numbers, but greater than zero. If the type supports subnormal values, `leastNonzeroMagnitude` is smaller than `leastNormalMagnitude`; otherwise they are equal.

