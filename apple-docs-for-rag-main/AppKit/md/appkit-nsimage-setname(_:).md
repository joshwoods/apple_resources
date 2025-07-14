

- AppKit
- NSImage
-  setName(\_:) 

Instance Method

# setName(\_:)

Registers the image object under the specified name.

macOS

``` source
func setName(_ string: NSImage.Name?) -> Bool
```

## Parameters 

`string`  

The name to associate with the receiver. Specify `nil` if you want to remove the image from the image cache.

## Return Value

true if the receiver was successfully registered with the given name; otherwise, false.

## Discussion

If the receiver is already registered under a different name, this method unregisters the other name. If a different image is already registered under the name specified in `aString`, this method does nothing and returns false.

When naming an image using this method, it is convention not to include filename extensions in the names you specify. That way, you can easily distinguish between images you have named explicitly and those you want to load from the app’s bundle. For information about the rules used to search for images, and for information about the ownership policy of named images, see the init(named:) method.

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

func name() -> NSImage.Name?

Returns the name associated with the image, if any.

typealias Name

Named images, defined by the system or you, for use in your app.

convenience init(imageLiteralResourceName: String)

Creates an image initialized with the specified resource name.

