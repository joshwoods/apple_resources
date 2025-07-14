

- AppKit
- NSPasteboard
-  releaseGlobally() 

Instance Method

# releaseGlobally()

Releases the receiver’s resources in the pasteboard server.

macOS

``` source
func releaseGlobally()
```

## Discussion

After this method is invoked, no other application can use the receiver.

Important

Although you must call this method to release a temporary, privately named pasteboard to avoid leaks, you should never call it on a standard pasteboard.

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

class func withUniqueName() -> NSPasteboard

Creates and returns a new pasteboard with a name that is guaranteed to be unique with respect to other pasteboards in the system.

