

- Core Image
- CIFilter
- CIRAWFilterOption
-  boostAmount Deprecated

Type Property

# boostAmount

A key for the amount of boost to apply to an image. The associated value is a floating-point value packaged as an NSNumber object. The value must be in the range of `0...1`. A value of `0` indicates no boost, that is, a linear response. The default value is `1`, which indicates full boost.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.5–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
static let boostAmount: CIRAWFilterOption
```

