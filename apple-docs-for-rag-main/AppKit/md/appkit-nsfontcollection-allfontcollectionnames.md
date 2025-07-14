

- AppKit
- NSFontCollection
-  allFontCollectionNames 

Type Property

# allFontCollectionNames

Returns all named collections visible to this process.

macOS 10.7+

``` source
class var allFontCollectionNames: [NSFontCollection.Name] { get }
```

## Return Value

`NSString` objects containing the names of all the named collections.

## See Also

### Naming the Font Collection

class func rename(fromName: NSFontCollection.Name, visibility: NSFontCollection.Visibility, toName: NSFontCollection.Name) throws

Renames the font collection with the specified name and visibility to the second name specified.

class func show(NSFontCollection, withName: NSFontCollection.Name, visibility: NSFontCollection.Visibility) throws

Make the given font collection visible by giving it a name.

class func hide(withName: NSFontCollection.Name, visibility: NSFontCollection.Visibility) throws

Remove from view the named font collection with the specified visibility.

struct Name

The constants represent the standard mutable collection names—these names are included in the list of allFontCollectionNames–they have special meaning to the Cocoa font system and should not be hidden or renamed.

struct Visibility

Constants that specify the visibility of font collections.

