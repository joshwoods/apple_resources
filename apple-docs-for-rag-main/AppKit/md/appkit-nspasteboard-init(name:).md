

- AppKit
- NSPasteboard
-  init(name:) 

Initializer

# init(name:)

Returns the pasteboard with the specified name.

macOS

``` source
init(name: NSPasteboard.Name)
```

## Parameters 

`name`  

The name of the pasteboard. The names of standard pasteboards are given in `Pasteboard Names`.

## Return Value

The pasteboard associated with the given name, or a new `NSPasteboard` object if the application does not yet have a pasteboard object for the specified name.

## Discussion

Other names can be assigned to create private pasteboards for other purposes.

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

struct Name

Constants that represent the standard pasteboard names.

class func withUniqueName() -> NSPasteboard

Creates and returns a new pasteboard with a name that is guaranteed to be unique with respect to other pasteboards in the system.

func releaseGlobally()

Releases the receiver’s resources in the pasteboard server.

