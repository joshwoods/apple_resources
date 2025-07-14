

- AppKit
- NSColor
-  NSColor.Name 

Type Alias

# NSColor.Name

The name of a color.

macOS

``` source
typealias Name = String
```

## See Also

### Loading Color Objects from Asset Catalogs

init?(named: NSColor.Name)

Creates a color object from the provided name, which corresponds to a color in the default asset catalog of the app’s main bundle.

init?(named: NSColor.Name, bundle: Bundle?)

Creates a color object from the provided name, which corresponds to a color in the default asset catalog of the specified bundle.

init?(catalogName: NSColorList.Name, colorName: NSColor.Name)

Creates a color object using the specified asset catalog and color names.

