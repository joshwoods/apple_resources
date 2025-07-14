

- Core Text
-  CTFontOptions 

Structure

# CTFontOptions

Options for font creation and descriptor matching.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CTFontOptions
```

## Overview

Use these options with the functions CTFontCreateWithNameAndOptions(_:_:_:_:) and CTFontCreateWithFontDescriptorAndOptions(_:_:_:_:).

## Topics

### Constants

static var preventAutoActivation: CTFontOptions

Prevents automatic font activation.

static var preferSystemFont: CTFontOptions

Font matching prefers to match Apple system fonts.

### Initializers

init(rawValue: CFOptionFlags)

Creates a font options structure with the specified raw value.

### Type Properties

static var preventAutoDownload: CTFontOptions

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

struct CTFontTableOptions

Constants that describe font table options.

