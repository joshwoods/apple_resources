

- AppKit
-  NSMutableFontCollection 

Class

# NSMutableFontCollection

A mutable collection of font descriptors taken together as a single object.

macOS 10.7+

``` source
class NSMutableFontCollection
```

## Overview

You can use this class to modify the search queries for the font descriptors used by the parent NSFontCollection class.

## Topics

### Creating a Font Collection

init(descriptors: [NSFontDescriptor])

Creates a mutable font collection containing the fonts that match the specified font descriptors.

init(locale: Locale)

Creates a mutable font collection containing fonts suitable for the specified locale.

init?(name: NSFontCollection.Name)

Creates a mutable named font collection object.

init?(name: NSFontCollection.Name, visibility: NSFontCollection.Visibility)

Creates a mutable font collection with the specified name and font visibility.

class var withAllAvailableDescriptors: NSMutableFontCollection

The mutable font collection that matches all registered fonts.

### Getting the Font Descriptors

var queryDescriptors: [NSFontDescriptor]?

The font descriptors to include in query results.

func addQuery(for: [NSFontDescriptor])

Edits the query and exclusion arrays by adding the specified font descriptors.

func removeQuery(for: [NSFontDescriptor])

Edits the query and exclusion arrays by removing the specified font descriptors.

var exclusionDescriptors: [NSFontDescriptor]?

The font descriptors to exclude from query results.

## Relationships

### Inherits From

- NSFontCollection

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol

## See Also

### Management

class NSFontManager

The center of activity for the font-conversion system.

class NSFontCollection

A font collection, which is a group of font descriptors taken together as a single object.

struct NSFontCollectionOptions

Constants that support font collection management.

