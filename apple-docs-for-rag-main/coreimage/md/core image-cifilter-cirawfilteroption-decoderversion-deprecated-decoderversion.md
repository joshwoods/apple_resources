

- Core Image
- CIFilter
- CIRAWFilterOption
-  decoderVersion Deprecated

Type Property

# decoderVersion

A key for the version number of the method to be used for decoding. A newly initialized object defaults to the newest available decoder version for the given image type. You can request an alternative, older version to maintain compatibility with older releases. Must be one of the values listed for the supportedDecoderVersions key, otherwise a `nil` output image is generated. The associated value must be an `NSNumber` object that specifies an integer value in range of `0` to the current decoder version. When you request a specific version of the decoder, Core Image produces an image that is *visually* the same across different versions of the operating system. Core Image, however, does not guarantee that the same bits are produced across different versions of the operating system. That’s because the rounding behavior of floating-point arithmetic can vary due to differences in compilers or hardware. Note that this option has no effect if the image used for initialization is not RAW.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.5–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
static let decoderVersion: CIRAWFilterOption
```

