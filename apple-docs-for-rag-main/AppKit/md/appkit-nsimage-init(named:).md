

- AppKit
- NSImage
-  init(named:) 

Initializer

# init(named:)

Returns the image object associated with the specified name.

macOS

``` source
init?(named name: NSImage.Name)
```

## Parameters 

`name`  

The name associated with the desired image. This can be a name you assigned to the image or the name of an image file in your app bundle.

## Return Value

The `NSImage` object associated with the specified name or `nil` if no such image was found.

## Discussion

This method searches for named images in several places, returning the first image it finds matching the given name. The order of the search is as follows:

1.  Search for an object whose name was set explicitly using the setName(_:) method and currently resides in the image cache.

2.  Search the app’s main bundle for a file whose name matches the specified string. (For information on how the bundle is searched, see “Accessing a Bundle’s Contents” in Bundle Programming Guide.)

3.  Search the Application Kit framework for a shared image with the specified name.

When looking for files in the app bundle, it is better (but not required) to include the filename extension in the `name` parameter. When naming an image with the setName(_:) method, it is convention not to include filename extensions in the names you specify. That way, you can easily distinguish between images you have named explicitly and those you want to load from the app’s bundle.

One particularly useful image you can retrieve is your app’s icon. This image is set by Cocoa automatically and accessible using the applicationIconName constant. Icons for other apps can be obtained through the use of methods declared in the NSWorkspace class. You can also retrieve many of the standard system images using Cocoa defined constants; for more information, see the `Image Template Constants`, `Sharing Permissions Named Images`, `System Entity Images`, `Toolbar Named Images`, and `View Type Template Images` sections for applicable constants.

If an app is linked on macOS 10.5 or later, images requested using this method and whose name ends in the word “Template” are automatically marked as template images.

The `NSImage` class may cache a reference to the returned image object for performance in some cases. However, the class holds onto cached objects only while the object exists. If all strong references to the image are subsequently removed, the object may be quietly removed from the cache. Thus, if you plan to hold onto a returned image object, you must maintain a strong reference to it like you would any Cocoa object. You can clear an image object from the cache explicitly by calling the object’s setName(_:) method and specifying `nil` for the image name.

## See Also

### Related Documentation

class func imageFileTypes() -> [String]

Returns an array of strings identifying the image types supported by the registered image representation objects.

Deprecated

func icon(forFile: String) -> NSImage

Returns an image containing the icon for the specified file.

### Creating Images by Name

Configuring and displaying symbol images in your UI

Create scalable images that integrate with your app’s text, and adjust the appearance of those images dynamically.

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

func name() -> NSImage.Name?

Returns the name associated with the image, if any.

typealias Name

Named images, defined by the system or you, for use in your app.

convenience init(imageLiteralResourceName: String)

Creates an image initialized with the specified resource name.

