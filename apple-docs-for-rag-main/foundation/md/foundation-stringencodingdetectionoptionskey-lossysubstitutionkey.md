

- Foundation
- StringEncodingDetectionOptionsKey
-  lossySubstitutionKey 

Type Property

# lossySubstitutionKey

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let lossySubstitutionKey: StringEncodingDetectionOptionsKey
```

## Discussion

Option specifying the string used to substitute for any unsupported characters when converting to a lossy string encoding. If a `@(NO)` value is specified for `NSStringEncodingDetectionAllowLossyKey`, this option has no effect. The corresponding value for this key is an `NSString` object. By default, this value is `U+FFFD`.

## See Also

### Type Properties

static let allowLossyKey: StringEncodingDetectionOptionsKey

static let disallowedEncodingsKey: StringEncodingDetectionOptionsKey

static let fromWindowsKey: StringEncodingDetectionOptionsKey

static let likelyLanguageKey: StringEncodingDetectionOptionsKey

static let suggestedEncodingsKey: StringEncodingDetectionOptionsKey

static let useOnlySuggestedEncodingsKey: StringEncodingDetectionOptionsKey

