

- AppKit
- NSPasteboard
- NSPasteboard.PasteboardType
-  URL 

Type Property

# URL

URL data for one file or resource.

macOS 10.13+

``` source
static let URL: NSPasteboard.PasteboardType
```

## Discussion

In macOS 10.6 and later, use writeObjects(_:) to write URLs directly to the pasteboard instead.

In macOS 10.5 and earlier, write an URL to a pasteboard using the write(to:) method of NSURL. To get an URL from a pasteboard, use the init(from:) method of NSURL.

## See Also

### Pasteboard Types

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

