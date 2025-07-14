

- Foundation
- StringEncodingDetectionOptionsKey
-  likelyLanguageKey 

Type Property

# likelyLanguageKey

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let likelyLanguageKey: StringEncodingDetectionOptionsKey
```

## Discussion

Option specifying the likely two-letter ISO 639-1 language code for the converted string. Use this when you have prior knowledge about the expected language of the converted string. The corresponding value for this key is an `NSString` object. If no value is specified, the language of the converted string is not considered.

## See Also

### Type Properties

static let allowLossyKey: StringEncodingDetectionOptionsKey

static let disallowedEncodingsKey: StringEncodingDetectionOptionsKey

static let fromWindowsKey: StringEncodingDetectionOptionsKey

static let lossySubstitutionKey: StringEncodingDetectionOptionsKey

static let suggestedEncodingsKey: StringEncodingDetectionOptionsKey

static let useOnlySuggestedEncodingsKey: StringEncodingDetectionOptionsKey

