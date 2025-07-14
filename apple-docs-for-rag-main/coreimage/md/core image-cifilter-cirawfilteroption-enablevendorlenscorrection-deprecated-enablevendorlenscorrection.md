

- Core Image
- CIFilter
- CIRAWFilterOption
-  enableVendorLensCorrection Deprecated

Type Property

# enableVendorLensCorrection

A key for whether to automatically correct for image distortion from known lenses.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.10–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
static let enableVendorLensCorrection: CIRAWFilterOption
```

## Discussion

The value for this key is a NSNumber object containing a Boolean value. If this value is `true`, or if this option is not specified but the image contains metadata for lens distortion parameters, Core Image corrects for lens distortion.

