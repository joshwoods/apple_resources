

- UIKit
- UIFontDescriptor
-  UIFontDescriptor.FeatureKey 

Structure

# UIFontDescriptor.FeatureKey

Keys for retrieving feature settings.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 4.0+

``` source
struct FeatureKey
```

## Overview

Use these keys when retrieving information from one of the dictionaries associated with the featureSettings key.

## Topics

### Keys

static let type: UIFontDescriptor.FeatureKey

A key for identifying the font feature type.

static let selector: UIFontDescriptor.FeatureKey

A key for identifying the font feature selector.

### Initializers

init(String)

Creates a font feature key.

init(rawValue: String)

Creates a font feature key with the specified raw value.

### Deprecated

static let featureIdentifier: UIFontDescriptor.FeatureKey

A key for identifying a font feature type.

Deprecated

static let typeIdentifier: UIFontDescriptor.FeatureKey

A key for identifying the font feature selector.

Deprecated

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

struct TraitKey

Keys for retrieving the font descriptor’s trait information.

struct Weight

Constants that represent standard typeface styles.

struct Width

