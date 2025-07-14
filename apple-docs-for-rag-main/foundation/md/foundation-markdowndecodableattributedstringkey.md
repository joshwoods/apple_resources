

- Foundation
-  MarkdownDecodableAttributedStringKey 

Protocol

# MarkdownDecodableAttributedStringKey

A protocol that defines how an attribute key decodes a value that corresponds to Markdown syntax.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol MarkdownDecodableAttributedStringKey : AttributedStringKey
```

## Overview

This protocol is separate from DecodableAttributedStringKey to separate explicit attributes defined by the SDK from Markdown’s semantic styling attributes. You use these attributes with Apple’s extended syntax for markdown: `^[text](attribute: value)`.

Using this protocol allows your markup names to differ from the names of your attributes. For example, the automatic grammar agreement feature uses markup like `^[text to inflect](inflect: true)`. This feature defines an AttributeScopes.FoundationAttributes.InflectionRuleAttribute that conforms to MarkdownDecodableAttributedStringKey. The value of its `AttributeScopes/FoundationAttributes/InflectionRuleAttribute/name` proprerty is `NSInflect`, while its `AttributeScopes/FoundationAttributes/InflectionRuleAttribute/markdownName-77fuy`, used in actual Markdown strings like the one shown here, is `inflect`.

To define your own attributes for use with Markdown syntax, make sure your attributes conform to this protocol. The markdown parser ignores attributes that don’t conform, even if you use the extended Markdown syntax.

Tip

When creating attributed strings from Markdown-based initializers like init(markdown:options:baseURL:), be sure to set the allowsExtendedAttributes option. If you don’t include this option, the string won’t parse MarkdownDecodableAttributedStringKey-based attributes.

## Topics

### Decoding Values

static func decodeMarkdown(from: any Decoder) throws -> Self.Value

Decodes a value from the provided decoder.

**Required** Default implementation provided.

### Accessing the Markdown Name

static var markdownName: String

The Markdown name associated with an attributed string key.

**Required** Default implementation provided.

## Relationships

### Inherits From

- AttributedStringKey

### Conforming Types

- AttributeScopes.AccessibilityAttributes.AdjustedPitchAttribute
- AttributeScopes.AccessibilityAttributes.AnnouncementPriorityAttribute
- AttributeScopes.AccessibilityAttributes.HeadingLevelAttribute
- AttributeScopes.AccessibilityAttributes.IPANotationAttribute
- AttributeScopes.AccessibilityAttributes.IncludesPunctuationAttribute
- AttributeScopes.AccessibilityAttributes.QueueAnnouncementAttribute
- AttributeScopes.AccessibilityAttributes.SpellOutAttribute
- AttributeScopes.AccessibilityAttributes.TextCustomAttribute
- AttributeScopes.AccessibilityAttributes.TextualContextAttribute
- AttributeScopes.FoundationAttributes.AgreementArgumentAttribute
- AttributeScopes.FoundationAttributes.AgreementConceptAttribute
- AttributeScopes.FoundationAttributes.InflectionAlternativeAttribute
- AttributeScopes.FoundationAttributes.InflectionRuleAttribute
- AttributeScopes.FoundationAttributes.LanguageIdentifierAttribute
- AttributeScopes.FoundationAttributes.LocalizedNumberFormatAttribute
- AttributeScopes.FoundationAttributes.MorphologyAttribute
- AttributeScopes.FoundationAttributes.ReferentConceptAttribute

