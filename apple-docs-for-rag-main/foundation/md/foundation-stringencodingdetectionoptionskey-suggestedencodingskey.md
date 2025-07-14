

- Foundation
- StringEncodingDetectionOptionsKey
-  suggestedEncodingsKey 

Type Property

# suggestedEncodingsKey

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let suggestedEncodingsKey: StringEncodingDetectionOptionsKey
```

## Discussion

Option specifying any suggested string encodings. Use this when you have prior knowledge about the likely or expected encoding. The corresponding value for this key is an `NSArray` of `NSNumber` objects that contain `NSStringEncoding` values. If this option is unspecified, all allowed encodings are evaluated with equal consideration.

## See Also

### Type Properties

static let allowLossyKey: StringEncodingDetectionOptionsKey

static let disallowedEncodingsKey: StringEncodingDetectionOptionsKey

static let fromWindowsKey: StringEncodingDetectionOptionsKey

static let likelyLanguageKey: StringEncodingDetectionOptionsKey

static let lossySubstitutionKey: StringEncodingDetectionOptionsKey

static let useOnlySuggestedEncodingsKey: StringEncodingDetectionOptionsKey

