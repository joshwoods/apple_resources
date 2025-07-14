

- AppKit
- NSFontManager
-  collectionNames Deprecated

Instance Property

# collectionNames

The names of the currently loaded font collections.

macOS 10.0–10.11Deprecated

``` source
var collectionNames: [Any] { get }
```

Deprecated

Use allFontCollectionNames instead.

## See Also

### Related Documentation

func fontDescriptors(inCollection: String) -> [Any]?

Returns an array of the font descriptors in the specified collection.

Deprecated

### Properties

static var applicationOnlyMask: NSFontCollectionOptions

Makes the collection available only to the application.

var delegate: AnyObject?

The font manager’s delegate.

Deprecated

