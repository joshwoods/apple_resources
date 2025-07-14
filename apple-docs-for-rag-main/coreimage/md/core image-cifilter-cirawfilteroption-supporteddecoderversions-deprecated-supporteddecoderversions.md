

- Core Image
- CIFilter
- CIRAWFilterOption
-  supportedDecoderVersions Deprecated

Type Property

# supportedDecoderVersions

A key for the supported decoder versions. The associated value is an NSArray object that contains all supported decoder versions for the given image type, sorted in increasingly newer order. Each entry is an NSDictionary object that contains key-value pairs. All entries represent a valid version identifier that can be passed as the `kCIDecoderVersion` value for the key `kCIDecoderMethodKey`. Version values are read-only; attempting to set this value raises an exception. Currently, the only defined key is `@"version"` which has as its value an NSString that uniquely describing a given decoder version. This string might not be suitable for user interface display..

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.5–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
static let supportedDecoderVersions: CIRAWFilterOption
```

