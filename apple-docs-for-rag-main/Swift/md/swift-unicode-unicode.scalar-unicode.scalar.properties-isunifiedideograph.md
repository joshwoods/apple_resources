

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.Properties
-  isUnifiedIdeograph 

Instance Property

# isUnifiedIdeograph

A Boolean value indicating whether the scalar is one of the unified CJK ideographs in the Unicode Standard.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isUnifiedIdeograph: Bool { get }
```

## Discussion

This property is false for CJK punctuation and symbols, as well as for compatibility ideographs (which canonically decompose to unified ideographs).

This property corresponds to the “Unified_Ideograph” property in the Unicode Standard.

