

- Foundation
-  EncodableAttributedStringKey 

Protocol

# EncodableAttributedStringKey

A protocol that defines how an attribute key encodes its value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol EncodableAttributedStringKey : AttributedStringKey
```

## Overview

Implement this protocol to make an attribute encodable. Encoding an AttributedString or AttributeContainer drops any attributes whose types don’t conform to this protocol.

## Topics

### Encoding Values

static func encode(Self.Value, to: any Encoder) throws

Encodes a value to the provided encoder.

**Required** Default implementations provided.

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
- AttributeScopes.AppKitAttributes.AdaptiveImageGlyphAttribute
- AttributeScopes.AppKitAttributes.AttachmentAttribute
- AttributeScopes.AppKitAttributes.BackgroundColorAttribute
- AttributeScopes.AppKitAttributes.BaselineOffsetAttribute
- AttributeScopes.AppKitAttributes.ExpansionAttribute
- AttributeScopes.AppKitAttributes.FontAttribute
- AttributeScopes.AppKitAttributes.ForegroundColorAttribute
- AttributeScopes.AppKitAttributes.GlyphInfoAttribute
- AttributeScopes.AppKitAttributes.KernAttribute
- AttributeScopes.AppKitAttributes.LigatureAttribute
- AttributeScopes.AppKitAttributes.MarkedClauseSegmentAttribute
- AttributeScopes.AppKitAttributes.ObliquenessAttribute
- AttributeScopes.AppKitAttributes.ParagraphStyleAttribute
- AttributeScopes.AppKitAttributes.ShadowAttribute
- AttributeScopes.AppKitAttributes.StrikethroughColorAttribute
- AttributeScopes.AppKitAttributes.StrikethroughStyleAttribute
- AttributeScopes.AppKitAttributes.StrokeColorAttribute
- AttributeScopes.AppKitAttributes.StrokeWidthAttribute
- AttributeScopes.AppKitAttributes.SuperscriptAttribute
- AttributeScopes.AppKitAttributes.TextAlternativesAttribute
- AttributeScopes.AppKitAttributes.TextEffectAttribute
- AttributeScopes.AppKitAttributes.ToolTipAttribute
- AttributeScopes.AppKitAttributes.TrackingAttribute
- AttributeScopes.AppKitAttributes.UnderlineColorAttribute
- AttributeScopes.AppKitAttributes.UnderlineStyleAttribute
- AttributeScopes.FoundationAttributes.AgreementArgumentAttribute
- AttributeScopes.FoundationAttributes.AgreementConceptAttribute
- AttributeScopes.FoundationAttributes.AlternateDescriptionAttribute
- AttributeScopes.FoundationAttributes.ByteCountAttribute
- AttributeScopes.FoundationAttributes.DateFieldAttribute
- AttributeScopes.FoundationAttributes.DurationFieldAttribute
- AttributeScopes.FoundationAttributes.ImageURLAttribute
- AttributeScopes.FoundationAttributes.InflectionAlternativeAttribute
- AttributeScopes.FoundationAttributes.InflectionRuleAttribute
- AttributeScopes.FoundationAttributes.InlinePresentationIntentAttribute
- AttributeScopes.FoundationAttributes.LanguageIdentifierAttribute
- AttributeScopes.FoundationAttributes.LinkAttribute
- AttributeScopes.FoundationAttributes.LocalizedNumberFormatAttribute
- AttributeScopes.FoundationAttributes.LocalizedStringArgumentAttributes.LocalizedDateArgumentAttribute
- AttributeScopes.FoundationAttributes.LocalizedStringArgumentAttributes.LocalizedDateIntervalArgumentAttribute
- AttributeScopes.FoundationAttributes.LocalizedStringArgumentAttributes.LocalizedNumericArgumentAttribute
- AttributeScopes.FoundationAttributes.LocalizedStringArgumentAttributes.LocalizedURLArgumentAttribute
- AttributeScopes.FoundationAttributes.MarkdownSourcePositionAttribute
- AttributeScopes.FoundationAttributes.MeasurementAttribute
- AttributeScopes.FoundationAttributes.MorphologyAttribute
- AttributeScopes.FoundationAttributes.NumberFormatAttributes.NumberPartAttribute
- AttributeScopes.FoundationAttributes.NumberFormatAttributes.SymbolAttribute
- AttributeScopes.FoundationAttributes.PersonNameComponentAttribute
- AttributeScopes.FoundationAttributes.PresentationIntentAttribute
- AttributeScopes.FoundationAttributes.ReferentConceptAttribute
- AttributeScopes.FoundationAttributes.ReplacementIndexAttribute
- AttributeScopes.SwiftUIAttributes.BaselineOffsetAttribute
- AttributeScopes.SwiftUIAttributes.KerningAttribute
- AttributeScopes.SwiftUIAttributes.TrackingAttribute
- AttributeScopes.UIKitAttributes.AdaptiveImageGlyphAttribute
- AttributeScopes.UIKitAttributes.AttachmentAttribute
- AttributeScopes.UIKitAttributes.BackgroundColorAttribute
- AttributeScopes.UIKitAttributes.BaselineOffsetAttribute
- AttributeScopes.UIKitAttributes.ExpansionAttribute
- AttributeScopes.UIKitAttributes.FontAttribute
- AttributeScopes.UIKitAttributes.ForegroundColorAttribute
- AttributeScopes.UIKitAttributes.KernAttribute
- AttributeScopes.UIKitAttributes.LigatureAttribute
- AttributeScopes.UIKitAttributes.ObliquenessAttribute
- AttributeScopes.UIKitAttributes.ParagraphStyleAttribute
- AttributeScopes.UIKitAttributes.ShadowAttribute
- AttributeScopes.UIKitAttributes.StrikethroughColorAttribute
- AttributeScopes.UIKitAttributes.StrikethroughStyleAttribute
- AttributeScopes.UIKitAttributes.StrokeColorAttribute
- AttributeScopes.UIKitAttributes.StrokeWidthAttribute
- AttributeScopes.UIKitAttributes.TextEffectAttribute
- AttributeScopes.UIKitAttributes.TextItemTagAttribute
- AttributeScopes.UIKitAttributes.TrackingAttribute
- AttributeScopes.UIKitAttributes.UnderlineColorAttribute
- AttributeScopes.UIKitAttributes.UnderlineStyleAttribute

## See Also

### Encoding and Decoding Keys

protocol DecodableAttributedStringKey

A protocol that defines how an attribute key decodes its value.

typealias CodableAttributedStringKey

A type alias used by attribute keys that are both encodable and decodable.

