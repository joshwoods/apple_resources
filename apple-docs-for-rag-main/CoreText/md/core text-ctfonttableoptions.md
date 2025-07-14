

- Core Text
-  CTFontTableOptions 

Structure

# CTFontTableOptions

Constants that describe font table options.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CTFontTableOptions
```

## Topics

### Constants

init(rawValue: UInt32)

Creates a font table options structure with the specified raw value.

static var excludeSynthetic: CTFontTableOptions

The font table excludes synthetic font data.

Deprecated

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Enumerations

enum CTFontUIFontType

Constants that represent the specific user-interface purpose to specify for font creation.

typealias CTFontTableTag

Font table tags provide access to font table data.

struct CTFontOptions

Options for font creation and descriptor matching.

