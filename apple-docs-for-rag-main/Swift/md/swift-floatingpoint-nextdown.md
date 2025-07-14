

- Swift
- FloatingPoint
-  nextDown 

Instance Property

# nextDown

The greatest representable value that compares less than this value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var nextDown: Self { get }
```

**Required** Default implementation provided.

## Discussion

For any finite value `x`, `x.nextDown` is less than `x`. For `nan` or `-infinity`, `x.nextDown` is `x` itself. The following special cases also apply:

- If `x` is `infinity`, then `x.nextDown` is `greatestFiniteMagnitude`.

- If `x` is `leastNonzeroMagnitude`, then `x.nextDown` is `0.0`.

- If `x` is zero, then `x.nextDown` is `-leastNonzeroMagnitude`.

- If `x` is `-greatestFiniteMagnitude`, then `x.nextDown` is `-infinity`.

## Default Implementations

### FloatingPoint Implementations

var nextDown: Self

The greatest representable value that compares less than this value.

