

- UIKit
- UIFont
-  UIFont.Weight 

Structure

# UIFont.Weight

Constants that represent standard typeface styles.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 4.0+

``` source
struct Weight
```

## Overview

Use system-defined constants as interchangeable values for weight. Each constant corresponds to a different value that indicates the weight of a font. Use these constants to specify the weight parameter in systemFont(ofSize:weight:). When providing a weight that doesn’t precisely match a font face in the family, the system locates a face that most closely matches the request.

Note

Font familyNames don’t include all system-defined font constants.

## Topics

### Using system-defined font weights

static let ultraLight: UIFont.Weight

The ultra-light font weight.

static let thin: UIFont.Weight

The thin font weight.

static let light: UIFont.Weight

The light font weight.

static let regular: UIFont.Weight

The regular font weight.

static let medium: UIFont.Weight

The medium font weight.

static let semibold: UIFont.Weight

The semibold font weight.

static let bold: UIFont.Weight

The bold font weight.

static let heavy: UIFont.Weight

The heavy font weight.

static let black: UIFont.Weight

The black font weight.

### Balancing the appearance of symbols and text

func symbolWeight() -> UIImage.SymbolWeight

Provides the corresponding symbol weight for this font weight.

### Initializers

init(CGFloat)

Creates a font weight.

init(rawValue: CGFloat)

Creates a font weight with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Comparable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating System Fonts

class func systemFont(ofSize: CGFloat) -> UIFont

Returns the font object for standard interface items in the specified size.

class func systemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the font object for standard interface items in the specified size and weight.

class func systemFont(ofSize: CGFloat, weight: UIFont.Weight, width: UIFont.Width) -> UIFont

struct Width

class func boldSystemFont(ofSize: CGFloat) -> UIFont

Returns the font object for standard interface items in boldface type in the specified size.

class func italicSystemFont(ofSize: CGFloat) -> UIFont

Returns the font object for standard interface items in italic type in the specified size.

class func monospacedSystemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the fixed-width font for standard interface text in the specified size.

class func monospacedDigitSystemFont(ofSize: CGFloat, weight: UIFont.Weight) -> UIFont

Returns the standard system font with all digits of consistent width.

