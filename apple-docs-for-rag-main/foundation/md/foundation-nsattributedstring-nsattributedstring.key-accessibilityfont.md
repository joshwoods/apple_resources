

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  accessibilityFont 

Type Property

# accessibilityFont

Font keys (`NSDictionary`).

macOS 10.0+

``` source
static let accessibilityFont: NSAttributedString.Key
```

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

static let accessibilityShadow: NSAttributedString.Key

Text shadow (`NSNumber` as a Boolean value).

