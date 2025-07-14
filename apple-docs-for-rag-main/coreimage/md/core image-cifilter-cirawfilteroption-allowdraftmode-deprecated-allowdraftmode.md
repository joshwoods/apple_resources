

- Core Image
- CIFilter
- CIRAWFilterOption
-  allowDraftMode Deprecated

Type Property

# allowDraftMode

A key for allowing draft mode. The associated value is a Boolean value packaged as an NSNumber object. It’s best not to use draft mode if the image needs to be drawn without draft mode at a later time, because changing the value from `true` to `false` is an expensive operation. If the optional scale factor is smaller than a certain value, additionally setting draft mode can improve image decoding speed without any perceivable loss of quality. However, turning on draft mode does not have any effect if the scale factor is not below this threshold.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.5–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
static let allowDraftMode: CIRAWFilterOption
```

