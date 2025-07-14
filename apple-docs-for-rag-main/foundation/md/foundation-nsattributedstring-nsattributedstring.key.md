

- Foundation
- NSAttributedString
-  NSAttributedString.Key 

Structure

# NSAttributedString.Key

The attributes you apply to ranges of characters in an attributed string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Key
```

## Discussion

The NSAttributedString.Key type defines the attributes you apply to ranges of characters in an attributed string. Some attributes provide information about how to render, lay out, or interpret the text, while other attributes provide transient or collaborative information. Attributes like the font, kern, and strokeColor contain information that the rendering system uses to display the text. Attributes like the spellingState, textHighlightStyle, or accessibilityCustomText contain semantic information from other parts of the system. Some of these semantic attributes also affect how the system renders the text, but they are transient attributes unlike the core rendering attributes.

## Topics

### Getting rendering attribute keys

static let backgroundColor: NSAttributedString.Key

The color of the background behind the text.

static let baselineOffset: NSAttributedString.Key

The vertical offset for the position of the text.

static let font: NSAttributedString.Key

The font of the text.

static let foregroundColor: NSAttributedString.Key

The color of the text.

static let glyphInfo: NSAttributedString.Key

The name of a glyph info object.

static let kern: NSAttributedString.Key

The kerning of the text.

static let ligature: NSAttributedString.Key

The ligature of the text.

static let paragraphStyle: NSAttributedString.Key

The paragraph style of the text.

static let strikethroughColor: NSAttributedString.Key

The color of the strikethrough.

static let strikethroughStyle: NSAttributedString.Key

The strikethrough style of the text.

static let strokeColor: NSAttributedString.Key

The color of the stroke.

static let strokeWidth: NSAttributedString.Key

The width of the stroke.

static let superscript: NSAttributedString.Key

The superscript of the text.

static let tracking: NSAttributedString.Key

The amount to modify the default tracking.

static let underlineColor: NSAttributedString.Key

The color of the underline.

static let underlineStyle: NSAttributedString.Key

The underline style of the text.

static let writingDirection: NSAttributedString.Key

The writing direction of the text.

### Getting text attribute keys

static let cursor: NSAttributedString.Key

The cursor object.

static let link: NSAttributedString.Key

The link for the text.

static let markedClauseSegment: NSAttributedString.Key

The index of the marked clause segment.

static let replacementIndex: NSAttributedString.Key

The replacement position associated with a format string specifier.

static let shadow: NSAttributedString.Key

The shadow of the text.

static let spellingState: NSAttributedString.Key

The spelling state of the text.

static let suggestionHighlight: NSAttributedString.Key

A highlight associated with a Spotlight suggestion.

static let textAlternatives: NSAttributedString.Key

The alternatives for the text.

static let textEffect: NSAttributedString.Key

An attribute that applies a text effect to the text.

static let textHighlightColorScheme: NSAttributedString.Key

The custom highlight color to apply to the text.

static let textHighlightStyle: NSAttributedString.Key

An attribute that adds a highlight color to the text to emphasize it.

static let textItemTag: NSAttributedString.Key

The name of a custom tag associated with a text item.

static let toolTip: NSAttributedString.Key

The tooltip text.

### Getting attachment attribute keys

static let adaptiveImageGlyph: NSAttributedString.Key

The adaptive image glyph for the text.

static let attachment: NSAttributedString.Key

The attachment for the text.

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

static let accessibilityShadow: NSAttributedString.Key

Text shadow (`NSNumber` as a Boolean value).

static let accessibilitySpeechAnnouncementPriority: NSAttributedString.Key

static let accessibilitySpeechIPANotation: NSAttributedString.Key

A key that indicates the pronunciation of a specific word or phrase, such as a proper name.

static let accessibilitySpeechLanguage: NSAttributedString.Key

A key that indicates the language to use when speaking a string.

static let accessibilitySpeechPitch: NSAttributedString.Key

A key that indicates the pitch to apply to spoken content.

static let accessibilitySpeechPunctuation: NSAttributedString.Key

A key that indicates whether to speak punctuation.

static let accessibilitySpeechQueueAnnouncement: NSAttributedString.Key

A key that indicates whether to queue an announcement behind existing speech or to interrupt it.

static let accessibilitySpeechSpellOut: NSAttributedString.Key

static let accessibilityTextCustom: NSAttributedString.Key

A key for specifying custom attributes to apply to the text.

static let accessibilityTextHeadingLevel: NSAttributedString.Key

A key for specifying the heading level of the text.

static let accessibilityStrikethrough: NSAttributedString.Key

Text strikethrough (`NSNumber` as a Boolean value).

static let accessibilityStrikethroughColor: NSAttributedString.Key

Text strikethrough color (`CGColorRef`).

static let accessibilitySuperscript: NSAttributedString.Key

Text superscript style (`NSNumber`). Values \> 0 are superscript; values \

static let accessibilityUnderline: NSAttributedString.Key

Text underline style (`NSNumber`).

static let accessibilityUnderlineColor: NSAttributedString.Key

Text underline color (`CGColorRef`).

static let UIAccessibilityTextAttributeContext: NSAttributedString.Key

### Getting Markdown attribute keys

static let inlinePresentationIntent: NSAttributedString.Key

An attribute that provides details for an inline Markdown element.

static let presentationIntentAttributeName: NSAttributedString.Key

An attribute that provides details for a block-level Markdown element.

static let markdownSourcePosition: NSAttributedString.Key

The position in a Markdown source string corresponding to some attributed text.

static let alternateDescription: NSAttributedString.Key

An alternate description for a URL or image.

static let imageURL: NSAttributedString.Key

The URL for an image in Markdown text.

### Getting translation-related attribute keys

static let languageIdentifier: NSAttributedString.Key

The language identifier associated with the range of text.

static let morphology: NSAttributedString.Key

An attribute that contains grammatical properties to apply to the text.

static let inflectionRule: NSAttributedString.Key

An attribute that tells the system how to apply grammar rules and other modifiers to the range of text.

static let inflectionAlternative: NSAttributedString.Key

The alternative translation for a string when no suitable inflection exists.

static let agreeWithArgument: NSAttributedString.Key

static let agreeWithConcept: NSAttributedString.Key

static let referentConcept: NSAttributedString.Key

static let localizedNumberFormat: NSAttributedString.Key

### Deprecated Keys

static let expansion: NSAttributedString.Key

The expansion factor of the text.

Deprecated

static let obliqueness: NSAttributedString.Key

The obliqueness of the text.

Deprecated

static let verticalGlyphForm: NSAttributedString.Key

The vertical glyph form of the text.

Deprecated

static let characterShapeAttributeName: NSAttributedString.Key

The character shape attribute.

Deprecated

static let usesScreenFontsDocumentAttribute: NSAttributedString.Key

The screen fonts attribute.

Deprecated

### Initializers

init(String)

Creates an attributed string key.

init(rawValue: String)

### Type Properties

static let writingToolsExclusionAttributeName: NSAttributedString.Key

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting text content attributes

struct TextHighlightStyle

Constants that specify the type of highlight to apply to text.

struct TextHighlightColorScheme

Constants that specify the highlight color to use with the text.

struct TextEffectStyle

Constants for the type of effect to apply to the text.

enum SpellingState

Constants for the spelling state attribute key.

struct NSUnderlineStyle

Constants for the underline style and strikethrough style attribute keys.

enum NSWritingDirectionFormatType

Constants for the writing direction attribute key.

