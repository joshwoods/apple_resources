

- Swift
- Float80
-  radix 

Type Property

# radix

The radix, or base of exponentiation, for a floating-point type.

macOS 10.10+

``` source
static var radix: Int { get }
```

## Discussion

The magnitude of a floating-point value `x` of type `F` can be calculated by using the following formula, where `**` is exponentiation:

```
x.significand * (F.radix ** x.exponent)
```

A conforming type may use any integer radix, but values other than 2 (for binary floating-point types) or 10 (for decimal floating-point types) are extraordinarily rare in practice.

