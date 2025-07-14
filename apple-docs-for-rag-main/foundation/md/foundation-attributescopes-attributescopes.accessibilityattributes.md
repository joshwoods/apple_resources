

- Foundation
- AttributeScopes
-  AttributeScopes.AccessibilityAttributes 

Structure

# AttributeScopes.AccessibilityAttributes

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct AccessibilityAttributes
```

## Topics

### Instance Properties

let accessibilityHeadingLevel: AttributeScopes.AccessibilityAttributes.HeadingLevelAttribute

let accessibilitySpeechAdjustedPitch: AttributeScopes.AccessibilityAttributes.AdjustedPitchAttribute

let accessibilitySpeechAnnouncementPriority: AttributeScopes.AccessibilityAttributes.AnnouncementPriorityAttribute

let accessibilitySpeechAnnouncementsQueued: AttributeScopes.AccessibilityAttributes.QueueAnnouncementAttributeDeprecated

let accessibilitySpeechIncludesPunctuation: AttributeScopes.AccessibilityAttributes.IncludesPunctuationAttribute

let accessibilitySpeechPhoneticNotation: AttributeScopes.AccessibilityAttributes.IPANotationAttribute

let accessibilitySpeechSpellsOutCharacters: AttributeScopes.AccessibilityAttributes.SpellOutAttribute

let accessibilityTextCustom: AttributeScopes.AccessibilityAttributes.TextCustomAttribute

let accessibilityTextualContext: AttributeScopes.AccessibilityAttributes.TextualContextAttribute

### Enumerations

enum AdjustedPitchAttribute

An attribute to adjust the pitch the spoken speech.

enum AnnouncementPriorityAttribute

An attribute to define the urgency of the announcement.

enum HeadingLevelAttribute

An attribute for the level of this heading.

enum IPANotationAttribute

An attribute to define the International Phonetic Alphabet representation for speech.

enum IncludesPunctuationAttribute

An attribute to define how punctuation should be spoken.

enum QueueAnnouncementAttribute

An attribute to define if speech announcements spoken by VoiceOver should be queued behind existing speech rather than interrupting speech in progress.

Deprecated

enum SpellOutAttribute

An attribute to define if each character should be spoken separately.

enum TextCustomAttribute

An attribute for custom, localized text attributes.

enum TextualContextAttribute

An attribute for the textual context.

## Relationships

### Conforms To

- AttributeScope
- DecodingConfigurationProviding
- EncodingConfigurationProviding

