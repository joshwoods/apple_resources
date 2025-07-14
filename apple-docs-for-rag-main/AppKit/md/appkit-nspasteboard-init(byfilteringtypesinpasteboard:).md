

- AppKit
- NSPasteboard
-  init(byFilteringTypesInPasteboard:) 

Initializer

# init(byFilteringTypesInPasteboard:)

Creates a new pasteboard object that supplies the specified pasteboard data in as many types as possible based on the available filter services.

macOS

``` source
init(byFilteringTypesInPasteboard pboard: NSPasteboard)
```

``` source
init(byFilteringTypesIn pboard: NSPasteboard)
```

## Parameters 

`pboard`  

The original pasteboard object.

## Return Value

The new pasteboard object. This method returns the object in the `pasteboard` parameter if the pasteboard was returned by one of the `pasteboardByFiltering...` methods. This prevents a pasteboard from being expanded multiple times.

## Discussion

This process can be thought of as expanding the pasteboard, because the new pasteboard generally contains more representations of the data than `pasteboard`.

This method only returns the original types and the types that can be created as a result of a single filter; the pasteboard does not have defined types that are the result of translation by multiple filters.

No filter service is invoked until the data is actually requested, so invoking this method is reasonably inexpensive.

## See Also

### Creating and Releasing a Pasteboard

class var general: NSPasteboard

The shared pasteboard object to use for general content.

init(byFilteringData: Data, ofType: NSPasteboard.PasteboardType)

Creates a new pasteboard object that supplies the specified data in as many types as possible based on the available filter services.

init(byFilteringFile: String)

Creates a new pasteboard object that supplies the specified file in as many types as possible based on the available filter services.

init(name: NSPasteboard.Name)

Returns the pasteboard with the specified name.

struct Name

Constants that represent the standard pasteboard names.

class func withUniqueName() -> NSPasteboard

Creates and returns a new pasteboard with a name that is guaranteed to be unique with respect to other pasteboards in the system.

func releaseGlobally()

Releases the receiver’s resources in the pasteboard server.

