

- Foundation
- StringEncodingDetectionOptionsKey
-  fromWindowsKey 

Type Property

# fromWindowsKey

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let fromWindowsKey: StringEncodingDetectionOptionsKey
```

## Discussion

Option specifying whether to consider string encodings corresponding to Windows codepage numbers. The corresponding value for this key is an `NSNumber` object containing a Boolean value. If `@(YES)`, Windows string encodings are removed from consideration. By default, this value is `@(NO)`.

## See Also

### Type Properties

static let allowLossyKey: StringEncodingDetectionOptionsKey

static let disallowedEncodingsKey: StringEncodingDetectionOptionsKey

static let likelyLanguageKey: StringEncodingDetectionOptionsKey

static let lossySubstitutionKey: StringEncodingDetectionOptionsKey

static let suggestedEncodingsKey: StringEncodingDetectionOptionsKey

static let useOnlySuggestedEncodingsKey: StringEncodingDetectionOptionsKey

