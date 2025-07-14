

- Foundation
- StringEncodingDetectionOptionsKey
-  useOnlySuggestedEncodingsKey 

Type Property

# useOnlySuggestedEncodingsKey

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let useOnlySuggestedEncodingsKey: StringEncodingDetectionOptionsKey
```

## Discussion

Option specifying whether to only consider suggested string encodings. Use this only if you specify a value for `NSStringEncodingDetectionSuggestedEncodingsKey`. The corresponding value for this key is an `NSNumber` object containing a Boolean value. By default, this value is `@(NO)`.

## See Also

### Type Properties

static let allowLossyKey: StringEncodingDetectionOptionsKey

static let disallowedEncodingsKey: StringEncodingDetectionOptionsKey

static let fromWindowsKey: StringEncodingDetectionOptionsKey

static let likelyLanguageKey: StringEncodingDetectionOptionsKey

static let lossySubstitutionKey: StringEncodingDetectionOptionsKey

static let suggestedEncodingsKey: StringEncodingDetectionOptionsKey

