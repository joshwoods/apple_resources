

- AppKit
-  NSFontAssetRequest 

Class

# NSFontAssetRequest

macOS 10.13+

``` source
class NSFontAssetRequest
```

## Topics

### Creating a Font Asset Request

init(fontDescriptors: [NSFontDescriptor], options: NSFontAssetRequest.Options)

struct Options

### Downloading a Font Asset

func download(withCompletionHandler: ((any Error)?) -> Bool)

var downloadedFontDescriptors: [NSFontDescriptor]

### Getting the Download Progress

var progress: Progress

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- ProgressReporting

## See Also

### Font Data

class NSFont

The representation of a font in an app.

class NSFontDescriptor

A dictionary of attributes that describe a font.

struct NSFontTraitMask

Constants for isolating specific traits of a font.

typealias NSFontFamilyClass

Constants that classify certain stylistic qualities of the font.

struct SymbolicTraits

A symbolic description of the stylistic aspects of a font.

typealias NSFontSymbolicTraits

A symbolic description of stylistic aspects of a font.

