

- UIKit
- UIFontDescriptor
-  UIFontDescriptor.SystemDesign 

Structure

# UIFontDescriptor.SystemDesign

Constants that describe the system-defined typeface designs.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 5.2+

``` source
struct SystemDesign
```

## Overview

Use these constants to specify a system-provided typeface design, such as:

- SF Pro in iOS or SF Compact in watchOS (default)

- SF Pro Rounded in iOS or SF Compact Rounded in watchOS (rounded)

- SF Mono (monospaced)

- New York (serif)

## Topics

### Typeface designs

static let `default`: UIFontDescriptor.SystemDesign

The default typeface for an app’s user interface.

static let rounded: UIFontDescriptor.SystemDesign

The rounded variant of the default typeface.

static let monospaced: UIFontDescriptor.SystemDesign

The monospace variant of the default typeface.

static let serif: UIFontDescriptor.SystemDesign

The serif variant of the default typeface.

### Initializers

init(rawValue: String)

Creates a typeface design constant with the specified raw value.

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

struct SymbolicTraits

Constants that describe the stylistic aspects of a font.

typealias Class

Constants that classify certain stylistic qualities of the font.

struct AttributeName

Constants that describe font attributes.

struct FeatureKey

Keys for retrieving feature settings.

struct TraitKey

Keys for retrieving the font descriptor’s trait information.

struct Weight

Constants that represent standard typeface styles.

struct Width

