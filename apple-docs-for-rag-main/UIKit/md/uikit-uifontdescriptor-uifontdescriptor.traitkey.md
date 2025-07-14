

- UIKit
- UIFontDescriptor
-  UIFontDescriptor.TraitKey 

Structure

# UIFontDescriptor.TraitKey

Keys for retrieving the font descriptor’s trait information.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 4.0+

``` source
struct TraitKey
```

## Overview

Use these keys to fetch values from the dictionary associated with the traits key.

## Topics

### Font traits

static let slant: UIFontDescriptor.TraitKey

The relative slant angle of the font.

static let symbolic: UIFontDescriptor.TraitKey

The symbolic font traits.

static let weight: UIFontDescriptor.TraitKey

The numerical value that corresponds to a font face.

static let width: UIFontDescriptor.TraitKey

The inter-glyph spacing of the font.

### Initializer

init(rawValue: String)

Creates a font trait key with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

struct TextStyle

Constants that describe the preferred styles for fonts.

struct SystemDesign

Constants that describe the system-defined typeface designs.

struct SymbolicTraits

Constants that describe the stylistic aspects of a font.

typealias Class

Constants that classify certain stylistic qualities of the font.

struct AttributeName

Constants that describe font attributes.

struct FeatureKey

Keys for retrieving feature settings.

struct Weight

Constants that represent standard typeface styles.

struct Width

