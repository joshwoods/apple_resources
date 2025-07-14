

- Swift
- SIMDMask
-  replace(with:where:) 

Instance Method

# replace(with:where:)

Replaces elements of this vector with `other` in the lanes where `mask` is `true`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func replace(
    with other: Self.Scalar,
    where mask: SIMDMask
)
```

## Discussion

Equivalent to:

```
for i in indices {
  if mask[i] { self[i] = other }
}
```

