

- AppKit
- NSImage
-  init(symbolName:variableValue:) 

Initializer

# init(symbolName:variableValue:)

Creates a symbol image with the symbol name and variable value you specify.

macOS 13.0+

``` source
convenience init?(
    symbolName name: String,
    variableValue value: Double
)
```

## Parameters 

`name`  

The name of the symbol image.

`value`  

The value the system uses to customize the symbol’s content, between `0` and `1`.

## Discussion

The `value` parameter is valid for symbols that support variable rendering.

## See Also

### Creating Images by Name

Configuring and displaying symbol images in your UI

Create scalable images that integrate with your app’s text, and adjust the appearance of those images dynamically.

init?(named: NSImage.Name)

Returns the image object associated with the specified name.

convenience init?(systemSymbolName: String, accessibilityDescription: String?)

Creates a symbol image with the system symbol name and accessibility description you specify.

convenience init?(systemSymbolName: String, variableValue: Double, accessibilityDescription: String?)

Creates a symbol image with the system symbol name and variable value you specify.

convenience init?(symbolName: String, bundle: Bundle?, variableValue: Double)

convenience init(resource: ImageResource)

func setName(NSImage.Name?) -> Bool

Registers the image object under the specified name.

func name() -> NSImage.Name?

Returns the name associated with the image, if any.

typealias Name

Named images, defined by the system or you, for use in your app.

convenience init(imageLiteralResourceName: String)

Creates an image initialized with the specified resource name.

