

- AppKit
- NSColor
-  init(named:) 

Initializer

# init(named:)

Creates a color object from the provided name, which corresponds to a color in the default asset catalog of the app’s main bundle.

macOS 10.13+

``` source
init?(named name: NSColor.Name)
```

## Parameters 

`name`  

The name of the color in the asset catalog.

## See Also

### Loading Color Objects from Asset Catalogs

init?(named: NSColor.Name, bundle: Bundle?)

Creates a color object from the provided name, which corresponds to a color in the default asset catalog of the specified bundle.

init?(catalogName: NSColorList.Name, colorName: NSColor.Name)

Creates a color object using the specified asset catalog and color names.

typealias Name

The name of a color.

