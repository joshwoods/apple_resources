

- AppKit
- NSFontCollection
-  NSFontCollection.Visibility 

Structure

# NSFontCollection.Visibility

Constants that specify the visibility of font collections.

macOS

``` source
struct Visibility
```

## Topics

### Visibility Options

static var process: NSFontCollection.Visibility

The font collection is visible within this process and is not persistent.

static var user: NSFontCollection.Visibility

The font collection is visible to all processes and is stored persistently.

static var computer: NSFontCollection.Visibility

The font collection is visible to all users and is stored persistently.

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

### Naming the Font Collection

class func rename(fromName: NSFontCollection.Name, visibility: NSFontCollection.Visibility, toName: NSFontCollection.Name) throws

Renames the font collection with the specified name and visibility to the second name specified.

class func show(NSFontCollection, withName: NSFontCollection.Name, visibility: NSFontCollection.Visibility) throws

Make the given font collection visible by giving it a name.

class func hide(withName: NSFontCollection.Name, visibility: NSFontCollection.Visibility) throws

Remove from view the named font collection with the specified visibility.

class var allFontCollectionNames: [NSFontCollection.Name]

Returns all named collections visible to this process.

struct Name

The constants represent the standard mutable collection names—these names are included in the list of allFontCollectionNames–they have special meaning to the Cocoa font system and should not be hidden or renamed.

