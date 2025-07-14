

- AppKit
-  NSFontCollectionOptions 

Structure

# NSFontCollectionOptions

Constants that support font collection management.

macOS

``` source
struct NSFontCollectionOptions
```

## Topics

### Options

static var applicationOnlyMask: NSFontCollectionOptions

Makes the collection available only to the application.

### Initializers

init(rawValue: UInt)

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

### Management

class NSFontManager

The center of activity for the font-conversion system.

class NSFontCollection

A font collection, which is a group of font descriptors taken together as a single object.

class NSMutableFontCollection

A mutable collection of font descriptors taken together as a single object.

