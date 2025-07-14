

- AppKit
- NSImage
-  name() 

Instance Method

# name()

Returns the name associated with the image, if any.

macOS

``` source
func name() -> NSImage.Name?
```

## Return Value

The name associated with the image, or `nil` if it has no associated name.

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

convenience init?(symbolName: String, variableValue: Double)

Creates a symbol image with the symbol name and variable value you specify.

convenience init?(symbolName: String, bundle: Bundle?, variableValue: Double)

convenience init(resource: ImageResource)

func setName(NSImage.Name?) -> Bool

Registers the image object under the specified name.

typealias Name

Named images, defined by the system or you, for use in your app.

convenience init(imageLiteralResourceName: String)

Creates an image initialized with the specified resource name.

