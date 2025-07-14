

- Foundation
- AttributeScopes
-  AttributeScopes.UIKitAttributes 

Structure

# AttributeScopes.UIKitAttributes

Attribute scopes that UIKit defines.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct UIKitAttributes
```

## Topics

### Using Color Attributes

let backgroundColor: AttributeScopes.UIKitAttributes.BackgroundColorAttribute

A property for accessing a background color attribute.

let foregroundColor: AttributeScopes.UIKitAttributes.ForegroundColorAttribute

A property for accessing a foreground color attribute.

### Using Font and Layout Attributes

let font: AttributeScopes.UIKitAttributes.FontAttribute

A property for accessing a font attribute.

let kern: AttributeScopes.UIKitAttributes.KernAttribute

A property for accessing a kerning attribute.

let ligature: AttributeScopes.UIKitAttributes.LigatureAttribute

A property for accessing a ligature attribute.

let tracking: AttributeScopes.UIKitAttributes.TrackingAttribute

A property for accessing a tracking attribute.

### Using Text Styling Attributes

let baselineOffset: AttributeScopes.UIKitAttributes.BaselineOffsetAttribute

A property for accessing a baseline offset attribute.

let obliqueness: AttributeScopes.UIKitAttributes.ObliquenessAttribute

A property for accessing an obliqueness attribute.

let paragraphStyle: AttributeScopes.UIKitAttributes.ParagraphStyleAttribute

A property for accessing a paragraph style attribute.

let shadow: AttributeScopes.UIKitAttributes.ShadowAttribute

A property for accessing a shadow attribute.

let strikethroughColor: AttributeScopes.UIKitAttributes.StrikethroughColorAttribute

A property for accessing a strikethrough color attribute.

let strikethroughStyle: AttributeScopes.UIKitAttributes.StrikethroughStyleAttribute

A property for accessing a strikethrough style attribute.

let strokeColor: AttributeScopes.UIKitAttributes.StrokeColorAttribute

A property for accessing a stroke color attribute.

let strokeWidth: AttributeScopes.UIKitAttributes.StrokeWidthAttribute

A property for accessing a stroke width attribute.

let textEffect: AttributeScopes.UIKitAttributes.TextEffectAttribute

A property for accessing a text effect attribute.

let underlineColor: AttributeScopes.UIKitAttributes.UnderlineColorAttribute

A property for accessing an underline color attribute.

let underlineStyle: AttributeScopes.UIKitAttributes.UnderlineStyleAttribute

A property for accessing an underline style attribute.

### Using Attachments and Expansions

let attachment: AttributeScopes.UIKitAttributes.AttachmentAttribute

A property for accessing an attachment attribute.

let expansion: AttributeScopes.UIKitAttributes.ExpansionAttribute

A property for accessing an expansion attribute.

### Using Foundation Attributes

let foundation: AttributeScopes.FoundationAttributes

A property for accessing attributes defined by the Foundation framework.

### Instance Properties

let accessibility: AttributeScopes.AccessibilityAttributes

let adaptiveImageGlyph: AttributeScopes.UIKitAttributes.AdaptiveImageGlyphAttribute

let textItemTag: AttributeScopes.UIKitAttributes.TextItemTagAttribute

### Enumerations

enum AdaptiveImageGlyphAttribute

enum AttachmentAttribute

enum BackgroundColorAttribute

enum BaselineOffsetAttribute

enum ExpansionAttribute

enum FontAttribute

enum ForegroundColorAttribute

enum KernAttribute

enum LigatureAttribute

enum ObliquenessAttribute

enum ParagraphStyleAttribute

enum ShadowAttribute

enum StrikethroughColorAttribute

enum StrikethroughStyleAttribute

enum StrokeColorAttribute

enum StrokeWidthAttribute

enum TextEffectAttribute

enum TextItemTagAttribute

enum TrackingAttribute

enum UnderlineColorAttribute

enum UnderlineStyleAttribute

## Relationships

### Conforms To

- AttributeScope
- DecodingConfigurationProviding
- EncodingConfigurationProviding

## See Also

### UIKit-Defined Attributes

var uiKit: AttributeScopes.UIKitAttributes.Type

A property for accessing the attribute scopes that UIKit defines.

