

- Foundation
- StringEncodingDetectionOptionsKey
-  disallowedEncodingsKey 

Type Property

# disallowedEncodingsKey

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let disallowedEncodingsKey: StringEncodingDetectionOptionsKey
```

## Discussion

Option specifying any string encodings not to be considered. The corresponding value for this key is an `NSArray` of `NSNumber` objects that contain `NSStringEncoding` values. If this option is unspecified, no additional string encodings are removed from consideration.

## See Also

### Type Properties

static let allowLossyKey: StringEncodingDetectionOptionsKey

static let fromWindowsKey: StringEncodingDetectionOptionsKey

static let likelyLanguageKey: StringEncodingDetectionOptionsKey

static let lossySubstitutionKey: StringEncodingDetectionOptionsKey

static let suggestedEncodingsKey: StringEncodingDetectionOptionsKey

static let useOnlySuggestedEncodingsKey: StringEncodingDetectionOptionsKey

