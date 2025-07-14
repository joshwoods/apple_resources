

- Foundation
-  AttributedStringKey 

Protocol

# AttributedStringKey

A type that defines an attribute’s name and type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol AttributedStringKey
```

## Overview

You don’t instantiate types that conform to this protocol. Rather, dynamic member lookup uses this type as the basis for looking up key paths on AttributedString subtypes when using an AttributeScope type parameter. When it also conforms to CodableAttributedStringKey, (or DecodableAttributedStringKey/EncodableAttributedStringKey if the type isn’t fully codable), the AttributedStringKey describes which attributes of an AttributedString support encoding or decoding.

Attribute owners — typically frameworks — declare a key like the following:

```
enum OutlineColorAttribute : AttributedStringKey {
    typealias Value = Color
    static let name = "OutlineColor"
}
```

Callers can use these types to get attribute values from attributed strings, but typically you want to reference them by name. Attribute owners enable this by creating one or more structures that conform to AttributeScope, in which they provide short names for their attributes that map to the AttributedStringKey type. The following example shows how to do this:

```
struct MyTextStyleAttributes : AttributeScope {
    let outlineColor : OutlineColorAttribute // OutlineColorAttribute.Value == Color
    let shadowColor : ShadowColorAttribute // ShadowColorAttribute.Value == Color
    // etc.
}
```

After you extend AttributeScope like this, extend AttributeDynamicLookup to allow callers to use dynamic member lookup syntax, like `myAttributedString.outlineColor = .red`.

## Topics

### Delcaring Key Properties

static var name: String

The name of the key.

**Required**

associatedtype Value : Hashable

The type of the key’s value.

**Required**

### Describing the Key

var description: String

### Type Properties

static var inheritedByAddedText: Bool

**Required** Default implementation provided.

static var invalidationConditions: Set&lt;AttributedString.AttributeInvalidationCondition>?

**Required** Default implementation provided.

static var runBoundaries: AttributedString.AttributeRunBoundaries?

**Required** Default implementation provided.

## Relationships

### Inherited By

- DecodableAttributedStringKey
- EncodableAttributedStringKey
- MarkdownDecodableAttributedStringKey
- ObjectiveCConvertibleAttributedStringKey

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
- AttributeScopes.AppKitAttributes.CursorAttribute
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
- AttributeScopes.SwiftUIAttributes.AdaptiveImageGlyphAttribute
- AttributeScopes.SwiftUIAttributes.BackgroundColorAttribute
- AttributeScopes.SwiftUIAttributes.BaselineOffsetAttribute
- AttributeScopes.SwiftUIAttributes.FontAttribute
- AttributeScopes.SwiftUIAttributes.ForegroundColorAttribute
- AttributeScopes.SwiftUIAttributes.KerningAttribute
- AttributeScopes.SwiftUIAttributes.StrikethroughStyleAttribute
- AttributeScopes.SwiftUIAttributes.TrackingAttribute
- AttributeScopes.SwiftUIAttributes.UnderlineStyleAttribute
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

### Accessing Attributes

subscript&lt;T>(T.Type) -> T.Value?

Returns the attribute that corresponds to a specified key.

subscript&lt;K>(dynamicMember _: KeyPath&lt;AttributeDynamicLookup, K>) -> K.Value?

Returns the attribute that corresponds to a specified key path.

subscript&lt;S>(dynamicMember _: KeyPath&lt;AttributeScopes, S.Type>) -> ScopedAttributeContainer&lt;S>

Returns the attribute container that corresponds to a specified key path.

subscript&lt;K>(dynamicMember _: KeyPath&lt;AttributeDynamicLookup, K>) -> AttributeContainer.Builder&lt;K>

Returns a modified attribute container as part of building a chain of attributes.

static subscript&lt;K>(dynamicMember _: KeyPath&lt;AttributeDynamicLookup, K>) -> AttributeContainer.Builder&lt;K>

Returns a modified attribute container as part of building a chain of attributes, for use as a static method.

struct Builder

A type that iteratively builds attribute containers by setting attribute values.

