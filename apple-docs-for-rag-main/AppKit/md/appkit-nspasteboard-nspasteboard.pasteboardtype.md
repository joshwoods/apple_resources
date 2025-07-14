

- AppKit
- NSPasteboard
-  NSPasteboard.PasteboardType 

Structure

# NSPasteboard.PasteboardType

The supported pasteboard types.

macOS

``` source
struct PasteboardType
```

## Topics

### Pasteboard Types

static let URL: NSPasteboard.PasteboardType

URL data for one file or resource.

static let collaborationMetadata: NSPasteboard.PasteboardType

An object you use for conveying data during a collaboration.

static let color: NSPasteboard.PasteboardType

Color data.

static let fileContents: NSPasteboard.PasteboardType

A representation of a file’s contents.

static let fileURL: NSPasteboard.PasteboardType

A file URL.

static let findPanelSearchOptions: NSPasteboard.PasteboardType

Type for the find panel metadata property list.

static let font: NSPasteboard.PasteboardType

Font and character information.

static let html: NSPasteboard.PasteboardType

Type for HTML content.

static let multipleTextSelection: NSPasteboard.PasteboardType

Multiple text selection.

static let pdf: NSPasteboard.PasteboardType

PDF data.

static let png: NSPasteboard.PasteboardType

PNG image data.

static let rtf: NSPasteboard.PasteboardType

Rich Text Format (RTF) data.

static let rtfd: NSPasteboard.PasteboardType

RTFD formatted file contents.

static let ruler: NSPasteboard.PasteboardType

Paragraph formatting information.

static let sound: NSPasteboard.PasteboardType

Sound data.

static let string: NSPasteboard.PasteboardType

String data.

static let tabularText: NSPasteboard.PasteboardType

Tab-separated fields of text.

static let textFinderOptions: NSPasteboard.PasteboardType

Type for the Find panel metadata property list.

static let tiff: NSPasteboard.PasteboardType

Tag Image File Format (TIFF) data.

### Option Keys

struct FindPanelSearchOptionKey

Search options for the find panel.

struct TextFinderOptionKey

Search options for text in Finder.

### Initializers

init(String)

init(rawValue: String)

### Deprecated

static let filePromise: NSPasteboard.PasteboardType

Promised files.

Deprecated

static let inkText: NSPasteboard.PasteboardType

Ink text data.

Deprecated

static let postScript: NSPasteboard.PasteboardType

Encapsulated PostScript (EPS) code.

Deprecated

static let vCard: NSPasteboard.PasteboardType

VCard data.

Deprecated

var representedPathExtension: String?

A file type based on the passed pasteboard type.

Deprecated

static func fileContentsType(forPathExtension: String) -> NSPasteboard.PasteboardType!

Returns a pasteboard type based on the passed file type.

Deprecated

static func fileNameType(forPathExtension: String) -> NSPasteboard.PasteboardType!

Returns a pasteboard type based on the passed file type.

Deprecated

static func representedPathExtensions(from: [NSPasteboard.PasteboardType]) -> [String]?

Returns an array of file types based on the passed pasteboard types.

Deprecated

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Writing Data

func clearContents() -> Int

Clears the existing contents of the pasteboard.

func writeObjects([any NSPasteboardWriting]) -> Bool

Writes an array of objects to the receiver.

func setData(Data?, forType: NSPasteboard.PasteboardType) -> Bool

Sets the data as the representation for the specified type for the first item on the receiver.

func setPropertyList(Any, forType: NSPasteboard.PasteboardType) -> Bool

Sets the given property list as the representation for the specified type for the first item on the receiver.

func setString(String, forType: NSPasteboard.PasteboardType) -> Bool

Sets the given string as the representation for the specified type for the first item on the receiver.

