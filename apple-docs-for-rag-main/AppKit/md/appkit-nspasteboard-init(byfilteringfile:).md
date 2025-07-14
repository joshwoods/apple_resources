

- AppKit
- NSPasteboard
-  init(byFilteringFile:) 

Initializer

# init(byFilteringFile:)

Creates a new pasteboard object that supplies the specified file in as many types as possible based on the available filter services.

macOS

``` source
init(byFilteringFile filename: String)
```

## Parameters 

`filename`  

The filename to put on the pasteboard.

## Return Value

The new pasteboard object.

## Discussion

No filter service is invoked until the data is actually requested, so invoking this method is reasonably inexpensive.

## See Also

### Creating and Releasing a Pasteboard

class var general: NSPasteboard

The shared pasteboard object to use for general content.

init(byFilteringData: Data, ofType: NSPasteboard.PasteboardType)

Creates a new pasteboard object that supplies the specified data in as many types as possible based on the available filter services.

init(byFilteringTypesInPasteboard: NSPasteboard)

Creates a new pasteboard object that supplies the specified pasteboard data in as many types as possible based on the available filter services.

init(name: NSPasteboard.Name)

Returns the pasteboard with the specified name.

struct Name

Constants that represent the standard pasteboard names.

class func withUniqueName() -> NSPasteboard

Creates and returns a new pasteboard with a name that is guaranteed to be unique with respect to other pasteboards in the system.

func releaseGlobally()

Releases the receiver’s resources in the pasteboard server.

