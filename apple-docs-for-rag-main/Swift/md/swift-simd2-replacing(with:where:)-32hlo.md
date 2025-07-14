

- Swift
- SIMD2
-  replacing(with:where:) 

Instance Method

# replacing(with:where:)

Returns a copy of this vector, with elements replaced by elements of `other` in the lanes where `mask` is `true`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func replacing(
    with other: Self,
    where mask: SIMDMask
) -> Self
```

## Discussion

Equivalent to:

```
var result = Self()
for i in indices {
  result[i] = mask[i] ? other[i] : self[i]
}
```

