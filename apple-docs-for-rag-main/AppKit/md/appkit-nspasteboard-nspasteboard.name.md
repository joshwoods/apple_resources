

- AppKit
- NSPasteboard
-  NSPasteboard.Name 

Structure

# NSPasteboard.Name

Constants that represent the standard pasteboard names.

macOS

``` source
struct Name
```

## Topics

### Named Pasteboards

static let drag: NSPasteboard.Name

The pasteboard that stores data to move as the result of a drag operation.

static let find: NSPasteboard.Name

The pasteboard that holds information about the current state of the active application’s find panel.

static let font: NSPasteboard.Name

The pasteboard that holds font and character information and supports Copy Font and Paste Font commands that the text editor may implement.

static let general: NSPasteboard.Name

The pasteboard you use to perform ordinary cut, copy, and paste operations.

static let ruler: NSPasteboard.Name

The pasteboard that holds information about paragraph formats and supports the Copy Ruler and Paste Ruler commands that the text editor may implement.

### Deprecated

static let dragPboard: NSPasteboard.Name

The pasteboard that stores data to be moved as the result of a drag operation.

Deprecated

static let findPboard: NSPasteboard.Name

The pasteboard that holds information about the current state of the active application’s find panel.

Deprecated

static let fontPboard: NSPasteboard.Name

The pasteboard that holds font and character information and supports Copy Font and Paste Font commands that may be implemented in a text editor.

Deprecated

static let generalPboard: NSPasteboard.Name

The pasteboard used for ordinary cut, copy, and paste operations.

Deprecated

static let rulerPboard: NSPasteboard.Name

The pasteboard that holds information about paragraph formats and supports the Copy Ruler and Paste Ruler commands implemented in a text editor.

Deprecated

### Initializers

init(String)

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

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

class func withUniqueName() -> NSPasteboard

Creates and returns a new pasteboard with a name that is guaranteed to be unique with respect to other pasteboards in the system.

func releaseGlobally()

Releases the receiver’s resources in the pasteboard server.

