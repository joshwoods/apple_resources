

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.Properties
-  isDeprecated 

Instance Property

# isDeprecated

A Boolean value indicating whether the scalar is deprecated.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isDeprecated: Bool { get }
```

## Discussion

Scalars are never removed from the Unicode Standard, but the usage of deprecated scalars is strongly discouraged.

This property corresponds to the “Deprecated” property in the Unicode Standard.

