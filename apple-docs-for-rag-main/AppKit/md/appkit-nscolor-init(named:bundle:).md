

- AppKit
- NSColor
-  init(named:bundle:) 

Initializer

# init(named:bundle:)

Creates a color object from the provided name, which corresponds to a color in the default asset catalog of the specified bundle.

macOS 10.13+

``` source
init?(
    named name: NSColor.Name,
    bundle: Bundle?
)
```

## Parameters 

`name`  

The name of the color to find.

`bundle`  

The app bundle.

## See Also

### Loading Color Objects from Asset Catalogs

init?(named: NSColor.Name)

Creates a color object from the provided name, which corresponds to a color in the default asset catalog of the app’s main bundle.

init?(catalogName: NSColorList.Name, colorName: NSColor.Name)

Creates a color object using the specified asset catalog and color names.

typealias Name

The name of a color.

