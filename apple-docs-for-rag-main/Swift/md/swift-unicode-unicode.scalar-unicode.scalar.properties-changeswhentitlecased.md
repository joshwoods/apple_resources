

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.Properties
-  changesWhenTitlecased 

Instance Property

# changesWhenTitlecased

A Boolean value indicating whether the scalar’s normalized form differs from the `titlecaseMapping` of each constituent scalar.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var changesWhenTitlecased: Bool { get }
```

## Discussion

This property corresponds to the “Changes_When_Titlecased” property in the Unicode Standard.

