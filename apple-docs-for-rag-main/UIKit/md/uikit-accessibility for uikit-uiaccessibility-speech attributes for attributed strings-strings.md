

- UIKit
- Accessibility for UIKit
- UIAccessibility
-  Speech attributes for attributed strings 

API Collection

# Speech attributes for attributed strings

Apply attributes to text in an attributed string to modify the pronunciation of that text.

## Topics

### Constants

static let accessibilitySpeechPunctuation: NSAttributedString.Key

A key that indicates whether to speak punctuation.

static let accessibilitySpeechLanguage: NSAttributedString.Key

A key that indicates the language to use when speaking a string.

static let accessibilitySpeechPitch: NSAttributedString.Key

A key that indicates the pitch to apply to spoken content.

static let accessibilitySpeechQueueAnnouncement: NSAttributedString.Key

A key that indicates whether to queue an announcement behind existing speech or to interrupt it.

Deprecated

static let accessibilitySpeechIPANotation: NSAttributedString.Key

A key that indicates the pronunciation of a specific word or phrase, such as a proper name.

static let accessibilitySpeechAnnouncementPriority: NSAttributedString.Key

static let accessibilitySpeechSpellOut: NSAttributedString.Key

struct UIAccessibilityPriority

Constants that specify priorities for accessibility announcements.

## See Also

### Defining accessibility text and language

Text attributes for attributed strings

Apply attributes to text in an attributed string to convey extra information about the text.

@MainActor var accessibilityHeaderElements: [Any]? { get set }

@MainActor @NSCopying var accessibilityAttributedHint: NSAttributedString? { get set }

@MainActor @NSCopying var accessibilityAttributedLabel: NSAttributedString? { get set }

@MainActor var accessibilityLanguage: String? { get set }

@MainActor var accessibilityTextualContext: UIAccessibilityTextualContext? { get set }

@MainActor var accessibilityUserInputLabels: [String]! { get set }

@MainActor var accessibilityAttributedUserInputLabels: [NSAttributedString]! { get set }

@MainActor @NSCopying var accessibilityAttributedValue: NSAttributedString? { get set }

