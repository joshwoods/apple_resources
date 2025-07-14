

- Swift
- StaticString
-  hasPointerRepresentation 

Instance Property

# hasPointerRepresentation

A Boolean value that indicates whether the static string stores a pointer to a null-terminated sequence of UTF-8 code units.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var hasPointerRepresentation: Bool { get }
```

## Discussion

If `hasPointerRepresentation` is `false`, the static string stores a single Unicode scalar value.

