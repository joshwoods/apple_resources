

- AppKit
- NSImage
-  init(systemSymbolName:accessibilityDescription:) 

Initializer

# init(systemSymbolName:accessibilityDescription:)

Creates a symbol image with the system symbol name and accessibility description you specify.

macOS 11.0+

``` source
convenience init?(
    systemSymbolName name: String,
    accessibilityDescription description: String?
)
```

## Parameters 

`name`  

The name of the system symbol image.

`description`  

The accessibility description for the symbol image, if any.

## Return Value

A symbol image based on the name you specify; otherwise `nil` if the method couldn’t find a suitable image.

## Discussion

To look up the names of system symbol images, download the SF Symbols app from Apple Design Resources.

## See Also

### Creating Images by Name

Configuring and displaying symbol images in your UI

Create scalable images that integrate with your app’s text, and adjust the appearance of those images dynamically.

init?(named: NSImage.Name)

Returns the image object associated with the specified name.

convenience init?(systemSymbolName: String, variableValue: Double, accessibilityDescription: String?)

Creates a symbol image with the system symbol name and variable value you specify.

convenience init?(symbolName: String, variableValue: Double)

Creates a symbol image with the symbol name and variable value you specify.

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

