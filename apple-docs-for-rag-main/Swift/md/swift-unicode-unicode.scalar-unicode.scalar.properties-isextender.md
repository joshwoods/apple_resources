

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.Properties
-  isExtender 

Instance Property

# isExtender

A Boolean value indicating whether the scalar’s principal function is to extend the value or shape of a preceding alphabetic scalar.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isExtender: Bool { get }
```

## Discussion

Typical extenders are length and iteration marks.

This property corresponds to the “Extender” property in the Unicode Standard.

