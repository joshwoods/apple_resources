

- Swift
- StaticString
-  utf8Start 

Instance Property

# utf8Start

A pointer to a null-terminated sequence of UTF-8 code units.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var utf8Start: UnsafePointer { get }
```

## Discussion

Important

Accessing this property when `hasPointerRepresentation` is `false` triggers a runtime error.

