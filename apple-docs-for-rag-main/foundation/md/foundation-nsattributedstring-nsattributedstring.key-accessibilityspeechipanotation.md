

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  accessibilitySpeechIPANotation 

Type Property

# accessibilitySpeechIPANotation

A key that indicates the pronunciation of a specific word or phrase, such as a proper name.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
nonisolated
static let accessibilitySpeechIPANotation: NSAttributedString.Key
```

## Discussion

The value of this key is an NSString object that contains International Phonetic Alphabet (IPA) symbols.

## See Also

### Getting accessibility attribute keys

static let accessibilityAlignment: NSAttributedString.Key

static let accessibilityAnnotationTextAttribute: NSAttributedString.Key

static let accessibilityAttachment: NSAttributedString.Key

Text attachment (`id`).

Deprecated

static let accessibilityAutocorrected: NSAttributedString.Key

Autocorrected text (`NSNumber` as a Boolean value).

static let accessibilityBackgroundColor: NSAttributedString.Key

Text background color (`CGColorRef`).

static let accessibilityCustomText: NSAttributedString.Key

static let accessibilityFont: NSAttributedString.Key

Font keys (`NSDictionary`).

static let accessibilityForegroundColor: NSAttributedString.Key

Text foreground color (`CGColorRef`).

static let accessibilityLanguage: NSAttributedString.Key

static let accessibilityLink: NSAttributedString.Key

Text link (`id`).

static let accessibilityListItemIndex: NSAttributedString.Key

static let accessibilityListItemLevel: NSAttributedString.Key

static let accessibilityListItemPrefix: NSAttributedString.Key

static let accessibilityMarkedMisspelled: NSAttributedString.Key

Misspelled text that is visibly marked as misspelled (`NSNumber` as a Boolean value). If you’re implementing a custom text-editing app, use `NSAccessibilityMarkedMisspelledTextAttribute` to ensure that VoiceOver properly identifies misspelled text to users.

static let accessibilityMisspelled: NSAttributedString.Key

Misspelled text that isn’t necessarily visibly marked as misspelled (NSNumber as a Boolean value). Beginning in macOS 10.9, VoiceOver no longer checks for this attribute; instead, VoiceOver uses accessibilityMarkedMisspelled.

