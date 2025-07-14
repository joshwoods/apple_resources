

- AppKit
- NSPasteboard
- NSPasteboard.PasteboardType
-  string 

Type Property

# string

String data.

macOS 10.6+

``` source
static let string: NSPasteboard.PasteboardType
```

## Mentioned in 

Supporting Writing Tools via the pasteboard

## Discussion

Apps that adopt App Sandbox cannot access files identified using the string pasteboard type. Instead, use an NSURL object, a bookmark, or a filename pasteboard type.

## See Also

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

