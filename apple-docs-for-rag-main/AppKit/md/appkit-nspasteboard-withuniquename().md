

- AppKit
- NSPasteboard
-  withUniqueName() 

Type Method

# withUniqueName()

Creates and returns a new pasteboard with a name that is guaranteed to be unique with respect to other pasteboards in the system.

macOS

``` source
class func withUniqueName() -> NSPasteboard
```

## Return Value

The new pasteboard object.

## Discussion

This method is useful for apps that implement their own interprocess communication using pasteboards. Because the lifetime of a unique pasteboard is not related to the lifetime of the creating app, you must release a unique pasteboard by calling releaseGlobally() to avoid possible leaks.

## See Also

### Creating and Releasing a Pasteboard

class var general: NSPasteboard

The shared pasteboard object to use for general content.

init(byFilteringData: Data, ofType: NSPasteboard.PasteboardType)

Creates a new pasteboard object that supplies the specified data in as many types as possible based on the available filter services.

init(byFilteringFile: String)

Creates a new pasteboard object that supplies the specified file in as many types as possible based on the available filter services.

init(byFilteringTypesInPasteboard: NSPasteboard)

Creates a new pasteboard object that supplies the specified pasteboard data in as many types as possible based on the available filter services.

init(name: NSPasteboard.Name)

Returns the pasteboard with the specified name.

struct Name

Constants that represent the standard pasteboard names.

func releaseGlobally()

Releases the receiver’s resources in the pasteboard server.

