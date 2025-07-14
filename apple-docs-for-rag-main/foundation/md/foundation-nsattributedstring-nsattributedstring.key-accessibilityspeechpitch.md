

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  accessibilitySpeechPitch 

Type Property

# accessibilitySpeechPitch

A key that indicates the pitch to apply to spoken content.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
nonisolated
static let accessibilitySpeechPitch: NSAttributedString.Key
```

## Discussion

The value of this key is an NSNumber object that contains a floating-point value in the range of `0.0` to `2.0`. The value indicates whether to speak the text with a higher or lower pitch than the default. The default value for this attribute is `1.0`, which indicates a normal pitch. Values between `0.0` and `1.0` result in a lower pitch, and values between `1.0` and `2.0` result in a higher pitch.

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

