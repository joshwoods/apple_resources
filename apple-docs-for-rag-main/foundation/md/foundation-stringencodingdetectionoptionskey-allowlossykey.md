

- Foundation
- StringEncodingDetectionOptionsKey
-  allowLossyKey 

Type Property

# allowLossyKey

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let allowLossyKey: StringEncodingDetectionOptionsKey
```

## Discussion

Option specifying whether to allow lossy string conversion. The corresponding value for this key is an `NSNumber` object containing a Boolean value. If `@(NO)`, the a lossy string encoding may not be chosen. By default, this value is `@(YES)`.

## See Also

### Type Properties

static let disallowedEncodingsKey: StringEncodingDetectionOptionsKey

static let fromWindowsKey: StringEncodingDetectionOptionsKey

static let likelyLanguageKey: StringEncodingDetectionOptionsKey

static let lossySubstitutionKey: StringEncodingDetectionOptionsKey

static let suggestedEncodingsKey: StringEncodingDetectionOptionsKey

static let useOnlySuggestedEncodingsKey: StringEncodingDetectionOptionsKey

