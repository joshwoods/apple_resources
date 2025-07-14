

- AppKit
- NSPasteboard
-  general 

Type Property

# general

The shared pasteboard object to use for general content.

macOS

``` source
class var general: NSPasteboard { get }
```

## Return Value

The general pasteboard.

## Discussion

Invokes init(name:) to obtain the pasteboard.

## See Also

### Related Documentation

Drag and Drop Programming Topics

Pasteboard Programming Guide

Services Implementation Guide

### Creating and Releasing a Pasteboard

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

func releaseGlobally()

Releases the receiver’s resources in the pasteboard server.

