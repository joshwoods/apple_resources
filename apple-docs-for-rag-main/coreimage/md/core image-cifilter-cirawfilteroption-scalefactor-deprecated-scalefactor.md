

- Core Image
- CIFilter
- CIRAWFilterOption
-  scaleFactor Deprecated

Type Property

# scaleFactor

A key for the scale factor. The associated value is a floating-point value packaged as an NSNumber object that specifies the desired scale factor at which the image will be drawn. Setting this value can greatly improve the drawing performance. A value of `1` is the identity. In some cases, if you change the scale factor and enable draft mode, performance can decrease. See allowDraftMode.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.5–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
static let scaleFactor: CIRAWFilterOption
```

