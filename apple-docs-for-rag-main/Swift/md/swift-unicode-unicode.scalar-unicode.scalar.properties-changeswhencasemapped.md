

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.Properties
-  changesWhenCaseMapped 

Instance Property

# changesWhenCaseMapped

A Boolean value indicating whether the scalar may change when it undergoes case mapping.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var changesWhenCaseMapped: Bool { get }
```

## Discussion

This property is `true` whenever one or more of `changesWhenLowercased`, `changesWhenUppercased`, or `changesWhenTitlecased` are `true`.

This property corresponds to the “Changes_When_Casemapped” property in the Unicode Standard.

