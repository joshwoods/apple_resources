

- Swift
- Unicode
- Unicode.CanonicalCombiningClass
-  Unicode.CanonicalCombiningClass.RawValue 

Type Alias

# Unicode.CanonicalCombiningClass.RawValue

The raw type that can be used to represent all values of the conforming type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias RawValue = UInt8
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

