

- Swift
- FloatingPoint
-  radix 

Type Property

# radix

The radix, or base of exponentiation, for a floating-point type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var radix: Int { get }
```

**Required** Default implementation provided.

## Discussion

The magnitude of a floating-point value `x` of type `F` can be calculated by using the following formula, where `**` is exponentiation:

```
x.significand * (F.radix ** x.exponent)
```

A conforming type may use any integer radix, but values other than 2 (for binary floating-point types) or 10 (for decimal floating-point types) are extraordinarily rare in practice.

## Default Implementations

### FloatingPoint Implementations

static var radix: Int

The radix, or base of exponentiation, for a floating-point type.

