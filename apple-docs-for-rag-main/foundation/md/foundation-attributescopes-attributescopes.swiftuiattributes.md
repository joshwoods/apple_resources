

- Foundation
- AttributeScopes
-  AttributeScopes.SwiftUIAttributes 

Structure

# AttributeScopes.SwiftUIAttributes

Attribute scopes that SwiftUI defines.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct SwiftUIAttributes
```

## Topics

### Using Color Attributes

let backgroundColor: AttributeScopes.SwiftUIAttributes.BackgroundColorAttribute

A property for accessing a background color attribute.

let foregroundColor: AttributeScopes.SwiftUIAttributes.ForegroundColorAttribute

A property for accessing a foreground color attribute.

### Using Font and Layout Attributes

let font: AttributeScopes.SwiftUIAttributes.FontAttribute

A property for accessing a font attribute.

let tracking: AttributeScopes.SwiftUIAttributes.TrackingAttribute

A property for accessing a tracking attribute.

### Using Text Styling Attributes

let baselineOffset: AttributeScopes.SwiftUIAttributes.BaselineOffsetAttribute

A property for accessing a baseline offset attribute.

let kern: AttributeScopes.SwiftUIAttributes.KerningAttribute

A property for accessing a kerning attribute.

### Using Foundation Attributes

let foundation: AttributeScopes.FoundationAttributes

A property for accessing attributes defined by the Foundation framework.

### Instance Properties

let accessibility: AttributeScopes.AccessibilityAttributes

let adaptiveImageGlyph: AttributeScopes.SwiftUIAttributes.AdaptiveImageGlyphAttribute

let strikethroughStyle: AttributeScopes.SwiftUIAttributes.StrikethroughStyleAttribute

let underlineStyle: AttributeScopes.SwiftUIAttributes.UnderlineStyleAttribute

### Enumerations

enum AdaptiveImageGlyphAttribute

enum BackgroundColorAttribute

enum BaselineOffsetAttribute

enum FontAttribute

enum ForegroundColorAttribute

enum KerningAttribute

enum StrikethroughStyleAttribute

enum TrackingAttribute

enum UnderlineStyleAttribute

## Relationships

### Conforms To

- AttributeScope
- DecodingConfigurationProviding
- EncodingConfigurationProviding

## See Also

### SwiftUI-Defined Attributes

var swiftUI: AttributeScopes.SwiftUIAttributes.Type

A property for accessing the attribute scopes that SwiftUI defines.

