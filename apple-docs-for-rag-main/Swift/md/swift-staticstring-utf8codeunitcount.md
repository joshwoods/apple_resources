

- Swift
- StaticString
-  utf8CodeUnitCount 

Instance Property

# utf8CodeUnitCount

The number of UTF-8 code units (excluding the null terminator).

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var utf8CodeUnitCount: Int { get }
```

## Discussion

Important

Accessing this property when `hasPointerRepresentation` is `false` triggers a runtime error.

