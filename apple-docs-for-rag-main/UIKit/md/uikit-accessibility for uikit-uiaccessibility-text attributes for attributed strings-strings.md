

- UIKit
- Accessibility for UIKit
- UIAccessibility
-  Text attributes for attributed strings 

API Collection

# Text attributes for attributed strings

Apply attributes to text in an attributed string to convey extra information about the text.

## Topics

### Constants

static let accessibilityTextCustom: NSAttributedString.Key

A key for specifying custom attributes to apply to the text.

static let accessibilityTextHeadingLevel: NSAttributedString.Key

A key for specifying the heading level of the text.

static let UIAccessibilityTextAttributeContext: NSAttributedString.Key

## See Also

### Defining accessibility text and language

Speech attributes for attributed strings

Apply attributes to text in an attributed string to modify the pronunciation of that text.

@MainActor var accessibilityHeaderElements: [Any]? { get set }

@MainActor @NSCopying var accessibilityAttributedHint: NSAttributedString? { get set }

@MainActor @NSCopying var accessibilityAttributedLabel: NSAttributedString? { get set }

@MainActor var accessibilityLanguage: String? { get set }

@MainActor var accessibilityTextualContext: UIAccessibilityTextualContext? { get set }

@MainActor var accessibilityUserInputLabels: [String]! { get set }

@MainActor var accessibilityAttributedUserInputLabels: [NSAttributedString]! { get set }

@MainActor @NSCopying var accessibilityAttributedValue: NSAttributedString? { get set }

