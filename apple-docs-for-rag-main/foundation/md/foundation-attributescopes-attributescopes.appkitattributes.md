

- Foundation
- AttributeScopes
-  AttributeScopes.AppKitAttributes 

Structure

# AttributeScopes.AppKitAttributes

Attribute scopes that AppKit defines.

macOS 12.0+

``` source
struct AppKitAttributes
```

## Topics

### Using Color Attributes

let backgroundColor: AttributeScopes.AppKitAttributes.BackgroundColorAttribute

A property for accessing a background color attribute.

let foregroundColor: AttributeScopes.AppKitAttributes.ForegroundColorAttribute

A property for accessing a foreground color attribute.

### Using Font and Layout Attributes

let font: AttributeScopes.AppKitAttributes.FontAttribute

A property for accessing a font attribute.

let kern: AttributeScopes.AppKitAttributes.KernAttribute

A property for accessing a kerning attribute.

let ligature: AttributeScopes.AppKitAttributes.LigatureAttribute

A property for accessing a ligature attribute.

let glyphInfo: AttributeScopes.AppKitAttributes.GlyphInfoAttribute

A property for accessing a glyph information attribute.

let tracking: AttributeScopes.AppKitAttributes.TrackingAttribute

A property for accessing a tracking attribute.

### Using Text Styling Attributes

let baselineOffset: AttributeScopes.AppKitAttributes.BaselineOffsetAttribute

A property for accessing a baseline offset attribute.

let obliqueness: AttributeScopes.AppKitAttributes.ObliquenessAttribute

A property for accessing an obliqueness attribute.

Deprecated

let shadow: AttributeScopes.AppKitAttributes.ShadowAttribute

A property for accessing a shadow attribute.

let strikethroughColor: AttributeScopes.AppKitAttributes.StrikethroughColorAttribute

A property for accessing a strikethrough color attribute.

let strikethroughStyle: AttributeScopes.AppKitAttributes.StrikethroughStyleAttribute

A property for accessing a strikethrough style attribute.

let strokeColor: AttributeScopes.AppKitAttributes.StrokeColorAttribute

A property for accessing a stroke color attribute.

let strokeWidth: AttributeScopes.AppKitAttributes.StrokeWidthAttribute

A property for accessing a stroke width attribute.

let textEffect: AttributeScopes.AppKitAttributes.TextEffectAttribute

A property for accessing a text effect attribute.

let underlineColor: AttributeScopes.AppKitAttributes.UnderlineColorAttribute

A property for accessing an underline color attribute.

let underlineStyle: AttributeScopes.AppKitAttributes.UnderlineStyleAttribute

A property for accessing an underline style attribute.

### Using Attachments and Expansions

let attachment: AttributeScopes.AppKitAttributes.AttachmentAttribute

A property for accessing an attachment attribute.

let expansion: AttributeScopes.AppKitAttributes.ExpansionAttribute

A property for accessing an expansion attribute.

Deprecated

### Using User Interface Attributes

let cursor: AttributeScopes.AppKitAttributes.CursorAttribute

A property for accessing a cursor attribute.

let toolTip: AttributeScopes.AppKitAttributes.ToolTipAttribute

A property for accessing a tool tip attribute.

let textAlternatives: AttributeScopes.AppKitAttributes.TextAlternativesAttribute

A property for accessing a text alternatives attribute.

### Using Foundation Attributes

let foundation: AttributeScopes.FoundationAttributes

A property for accessing attributes defined by the Foundation framework.

### Using Text Layout and Presentation Attributes

let markedClauseSegment: AttributeScopes.AppKitAttributes.MarkedClauseSegmentAttribute

let paragraphStyle: AttributeScopes.AppKitAttributes.ParagraphStyleAttribute

let superscript: AttributeScopes.AppKitAttributes.SuperscriptAttribute

### Instance Properties

let accessibility: AttributeScopes.AccessibilityAttributes

let adaptiveImageGlyph: AttributeScopes.AppKitAttributes.AdaptiveImageGlyphAttribute

### Enumerations

enum AdaptiveImageGlyphAttribute

enum AttachmentAttribute

enum BackgroundColorAttribute

enum BaselineOffsetAttribute

enum CursorAttribute

enum ExpansionAttributeDeprecated

enum FontAttribute

enum ForegroundColorAttribute

enum GlyphInfoAttribute

enum KernAttribute

enum LigatureAttribute

enum MarkedClauseSegmentAttribute

enum ObliquenessAttributeDeprecated

enum ParagraphStyleAttribute

enum ShadowAttribute

enum StrikethroughColorAttribute

enum StrikethroughStyleAttribute

enum StrokeColorAttribute

enum StrokeWidthAttribute

enum SuperscriptAttribute

enum TextAlternativesAttribute

enum TextEffectAttribute

enum ToolTipAttribute

enum TrackingAttribute

enum UnderlineColorAttribute

enum UnderlineStyleAttribute

## Relationships

### Conforms To

- AttributeScope
- DecodingConfigurationProviding
- EncodingConfigurationProviding

## See Also

### AppKit-Defined Attributes

var appKit: AttributeScopes.AppKitAttributes.Type

A property for accessing the attribute scopes that AppKit defines.

