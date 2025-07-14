

- AppKit
- NSPasteboard
-  init(byFilteringData:ofType:) 

Initializer

# init(byFilteringData:ofType:)

Creates a new pasteboard object that supplies the specified data in as many types as possible based on the available filter services.

macOS

``` source
init(
    byFilteringData data: Data,
    ofType type: NSPasteboard.PasteboardType
)
```

## Parameters 

`data`  

The data to be placed on the pasteboard.

`type`  

The type of data in the `data` parameter.

## Return Value

The new pasteboard object.

## Discussion

The returned pasteboard also declares data of the supplied `type`.

No filter service is invoked until the data is actually requested, so invoking this method is reasonably inexpensive.

## See Also

### Creating and Releasing a Pasteboard

class var general: NSPasteboard

The shared pasteboard object to use for general content.

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

func releaseGlobally()

Releases the receiver’s resources in the pasteboard server.

