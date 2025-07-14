

- AppKit
- NSFontCollection
-  NSFontCollection.Name 

Structure

# NSFontCollection.Name

The constants represent the standard mutable collection names—these names are included in the list of allFontCollectionNames–they have special meaning to the Cocoa font system and should not be hidden or renamed.

macOS

``` source
struct Name
```

## Topics

### Type Properties

static let allFonts: NSFontCollection.Name

All fonts in the system.

static let user: NSFontCollection.Name

Per-user unmodifiable collection.

static let favorites: NSFontCollection.Name

Font collection of the user’s preferred font descriptors.

static let recentlyUsed: NSFontCollection.Name

Font collection automatically maintained by NSFontManager.

### Initializers

init(String)

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Naming the Font Collection

class func rename(fromName: NSFontCollection.Name, visibility: NSFontCollection.Visibility, toName: NSFontCollection.Name) throws

Renames the font collection with the specified name and visibility to the second name specified.

class func show(NSFontCollection, withName: NSFontCollection.Name, visibility: NSFontCollection.Visibility) throws

Make the given font collection visible by giving it a name.

class func hide(withName: NSFontCollection.Name, visibility: NSFontCollection.Visibility) throws

Remove from view the named font collection with the specified visibility.

class var allFontCollectionNames: [NSFontCollection.Name]

Returns all named collections visible to this process.

struct Visibility

Constants that specify the visibility of font collections.

