

- Swift
- SIMDMask
-  .^=(\_:\_:) 

Operator

# .^=(\_:\_:)

Replaces `a` with the pointwise exclusive or of `a` and `b`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func .^= (a: inout SIMDMask, b: SIMDMask)
```

Available when `Storage` is `SIMD4`.

## Discussion

Equivalent to:

```
for i in a.indices {
  a[i] = a[i] != b[i]
}
```

