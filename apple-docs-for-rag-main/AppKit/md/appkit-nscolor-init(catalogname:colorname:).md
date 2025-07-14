

- AppKit
- NSColor
-  init(catalogName:colorName:) 

Initializer

# init(catalogName:colorName:)

Creates a color object using the specified asset catalog and color names.

macOS

``` source
init?(
    catalogName listName: NSColorList.Name,
    colorName: NSColor.Name
)
```

## Parameters 

`listName`  

The name of the asset catalog in which to find the specified color; this may be a standard color catalog.

`colorName`  

The name of the color. Note that the color must be defined in the named color space to retrieve it with this method.

## Return Value

The color object.

## Discussion

This method searches the app’s main bundle for an asset catalog with the specified name. It then creates a color object based on the asset whose name matches the value in `colorName`.

## See Also

### Related Documentation

var catalogNameComponent: NSColorList.Name

The catalog containing the color’s name.

var localizedCatalogNameComponent: String

The localized version of the catalog name containing the color.

var colorNameComponent: NSColor.Name

The name of the color.

### Loading Color Objects from Asset Catalogs

init?(named: NSColor.Name)

Creates a color object from the provided name, which corresponds to a color in the default asset catalog of the app’s main bundle.

init?(named: NSColor.Name, bundle: Bundle?)

Creates a color object from the provided name, which corresponds to a color in the default asset catalog of the specified bundle.

typealias Name

The name of a color.

